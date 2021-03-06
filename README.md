[![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/zabirauf/ex_microsoftbot/master/LICENSE.md) [![hex.pm version](https://img.shields.io/hexpm/v/httpotion.svg?style=flat)](https://hex.pm/packages/ex_microsoftbot) [![Build Status](https://travis-ci.org/zabirauf/ex_microsoftbot.svg?branch=master)](https://travis-ci.org/zabirauf/ex_microsoftbot) [![Inline docs](http://inch-ci.org/github/zabirauf/ex_microsoftbot.svg)](http://inch-ci.org/github/zabirauf/ex_microsoftbot) <a href="http://github.com/syl20bnr/spacemacs"><img src="https://cdn.rawgit.com/syl20bnr/spacemacs/442d025779da2f62fc86c2082703697714db6514/assets/spacemacs-badge.svg" alt="Made with Spacemacs"></a>

# Elixir Microsoft Bot Client 

This library provides Elixir API wrapper for the Microsoft Bot Framework.

## Documentation

API documentation is available at [https://hexdocs.pm/ex_microsofbot](https://hexdocs.pm/ex_microsofbot)

## Installation

  1. Add `ex_microsoftbot` to your list of dependencies in `mix.exs`:

        def deps do
          [{:ex_microsoftbot, "~> 0.1.0"}]
        end
        
  2. Start the `ex_microsoftbot`:
  
        def application do
          [applications: [:ex_microsoftbot]]
        end
        
## Usage

The module `ExMicrosoftBot.Client` contains the functions to call the Microsoft bot API. For example

```
auth_data = %ExMicrosoftBot.Models.AuthData{app_id: "APPID", app_secret: "APP_SECRET"}

bot_data = ExMicrosoftBot.Client.get_user_data(auth_data, bot_id, user_id)

%ExMicrosoftBot.Models.BotData{data: %{}, eTag: "string"}
```
