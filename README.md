<br />

<p align="center">
  <img alt="Logo" src="./.github/logo.png" width="180px" />
</p>

<h1 align="center" style="text-align: center;">Parallelixir</h1>

<p align="center">
	<a href="https://github.com/LuizFerK">
		<img alt="Author" src="https://img.shields.io/badge/author-Luiz%20Fernando-5C0095?style=flat" />
	</a>
	<a href="#">
		<img alt="Languages" src="https://img.shields.io/github/languages/count/LuizFerK/Parallelixir?color=5C0095&style=flat" />
	</a>
	<a href="hhttps://github.com/LuizFerK/Parallelixir/stargazers">
		<img alt="Stars" src="https://img.shields.io/github/stars/LuizFerK/Parallelixir?color=5C0095&style=flat" />
	</a>
	<a href="https://github.com/LuizFerK/Parallelixir/network/members">
		<img alt="Forks" src="https://img.shields.io/github/forks/LuizFerK/Parallelixir?color=5C0095&style=flat" />
	</a>
	<a href="https://github.com/LuizFerK/Parallelixir/graphs/contributors">
		<img alt="Contributors" src="https://img.shields.io/github/contributors/LuizFerK/Parallelixir?color=5C0095&style=flat" />
	</a>
</p>

<p align="center">
	<b>Report of 300.000 lines in 0.4 seconds!</b><br />
	<span>Created with Elixir.</span><br />
	<sub>Made with ❤️</sub>
</p>

<br />

# :pushpin: Contents

- [Features](#rocket-features)
- [Installation](#wrench-installation)
- [Getting started](#bulb-getting-started)
- [Techs](#fire-techs)
- [Issues](#bug-issues)
- [License](#book-license)

# :rocket: Features

- Generate reports of 300,000 different food dishes
- Use of parallel processes to generate the report in up to 0.4 seconds
- Single process option (for comparisons) of up to 1.1 seconds

# :wrench: Installation

### Required :warning:
- Elixir
- Erlang

### SSH

SSH URLs provide access to a Git repository via SSH, a secure protocol. If you have an SSH key registered in your GitHub account, clone the project using this command:

```git clone git@github.com:LuizFerK/Parallelixir.git```

### HTTPS

In case you don't have an SSH key on your GitHub account, you can clone the project using the HTTPS URL, run this command:

```git clone https://github.com/LuizFerK/Parallelixir.git```

**Both of these commands will generate a folder called Parallelixir, with all the project**

# :bulb: Getting started

1. Run ```mix deps.get``` to install the dependencies
2. This project does not have a server, in this case, the mode of use is through IEx (Elixir's interactive shell), which can be accessed using the command ```iex -S mix``` in the project folder
3. Within IEx, you have two usage options: standard execution (which will run 300 thousand lines in just one process) and parallel execution (which will run 3 files of 100.000 lines simultaneously). To use the standard mode, run the following command:
> ReportsGenerator.build("report_complete.csv")
4. If you want to use the parallel mode, run the following command:
> ReportsGenerator.build_from_many(["report_1.csv", "report_2.csv", "report_3.csv"])
5. In both modes, you will have the same result, however, parallel execution will be faster
6. The result will be a **map** with the following information: ```foods``` (representing the total times that every food appears in the files) and ```users``` (representing the total times that every user appears in the files), as you can see below:
```elixir
{:ok,
 %{
   "foods" => %{
     "açaí" => 37742,
     "churrasco" => 37650,
     "esfirra" => 37462,
     "hambúrguer" => 37577,
     "pastel" => 37392,
     "pizza" => 37365,
     "prato_feito" => 37519,
     "sushi" => 37293
   },
   "users" => %{
     "1" => 278849,
     "10" => 268317,
     "11" => 268877,
     "12" => 276306,
     "13" => 282953,
     "14" => 277084,
     "15" => 280105,
     "16" => 271831,
     "17" => 272883,
     "18" => 271421,
     "19" => 277720,
     "2" => 271031,
     "20" => 273446,
     "21" => 275026,
     "22" => 278025,
     "23" => 276523,
     "24" => 274481,
     "25" => 274512,
     "26" => 274199,
     "27" => 278001,
     "28" => 274256,
     "29" => 273030,
     "3" => 272250,
     "30" => 275978,
     "4" => 277054,
     "5" => 270926,
     "6" => 272053,
     "7" => 273112,
     "8" => 275161,
     "9" => 274003
   }
 }}
```

# :fire: Techs

### Elixir
- Tasks

# :bug: Issues

Find a bug or error on the project? Please, feel free to send me the issue on the [Parallelixir issues area](https://github.com/LuizFerK/Parallelixir/issues), with a title and a description of your found!

If you know the origin of the error and know how to resolve it, please, send me a pull request, I will love to review it!

# :book: License

Released in 2020.

This project is under the [MIT license](https://github.com/LuizFerK/Parallelixir/blob/main/LICENSE).

<p align="center">
	< keep coding /> :rocket: :heart:
</p>
