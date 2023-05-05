# Pokemon Chat Bot with kata platform & pokeapi

Kata Platform is a tool to build the conversational AI product from start to finish.
Pokeapi is a full RESTful API linked to an extensive database detailing everything

## Features

- Kata Platform : https://platform.kata.ai
- Poke api : https://pokeapi.co/
- Telegram Chat Bot : BotFather
- Pokemon Information : Name, Type, Weight, Height, and Picture

## Registration
- Open your browser and enter the URL https://platform.kata.ai/.
- Register your data in the Kata Platform by filling in the required fields.

## Installation

We are using Kata Command Line Interface (Kata CLI) is a tool for creating bot with Kata Markup Language (Kata ML) and helps managing the bots with command line/shell of various operating systems.

Install Kata-CLI using the npm package manager.

```sh
npm install -g kata-cli
```

Login to Kata-CLI

```sh
kata login [options]
```

Create New Project
```sh
kata create-project [project name]
```

Select project that you want to use, any bot operation will be related to that project
```sh
kata select-project [project name]
```

Initialize the bot
```sh
kata init <botName>
```
It will create a bot file with default YAML template.
```sh
bot.yml
```
Replace the content of the default bot.yml with the new bot.yml consist of the Poke Bot

Push the new bot.yml to Kata Platform
```sh
kata push
```

## pokeapi endpoints

We can use these endpoint to get specific information from the API


| value | endpoint |
| ------ | ------ |
| name/id | https://pokeapi.co/api/v2/pokemon/{id or name}/ |
| weight | (result.weight) |
| height | (result.height) |
| image | https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/$(result.id).png |

