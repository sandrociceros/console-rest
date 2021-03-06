# Console.REST

[![Slack Status](https://console-rest-slackin.herokuapp.com/badge.svg)](https://console-rest-slackin.herokuapp.com)

Console.REST is a converter service for API description formats and HTTP clients, such as Swagger, RAML, Curl, Postman, and Paw.

This project is open-source, and can be used in multiple ways:
- as a client-side web service, at [https://console.rest/](https://console.rest).
- as a button present on the documentation of API providers.
- as a Chrome extension for users to use on popular API documentations, based on [apis.guru](https://apis.guru) (Still in development).
- as a JS library that allows users to programmatically convert formats.

## Dependencies

Console.REST uses the open-source library [API-Flow](https://github.com/luckymarmot/API-Flow) to convert between formats. As a standalone, API-Flow is available as a webworker, a web library, and a node module.

## Button

Console.REST provides API providers with 2 snippets to plug into their API docs to allow their users to download them in their preferred format:
- An HTML/JS Snippet for web documentation, that injects itself in the context of the page to give a seamless experience to the user.
- A Markdown Snippet for github documentation, that uses Console.REST as a Service.

The button looks like this

[![Run API With...](https://console.rest/github.io/assets/buttons/run_with_red.svg)](https://console.rest/#?name=swagger&format=swagger&version=v2.0&uri=https%3A%2F%2Fapi.apis.guru%2Fv2%2Fspecs%2Fxkcd.com%2F1.0.0%2Fswagger.yaml)

You can read more about how to use the button in your API documentation in the [wiki](https://github.com/luckymarmot/console-rest/wiki).

## URL Scheme

[Console.REST](https://console.rest) exposes a simple API that allows anyone to open it with a file to convert. You can find more information on the API in the [wiki](https://github.com/luckymarmot/console-rest/wiki/window.location.hash).

## JS Library

A stripped down version of Console.REST without any of the visuals is also available for users and API providers that want to integrate the functionalities of Console.REST and API-Flow even further into their projects.

You can read more about the API of the JS library in the [wiki](https://github.com/luckymarmot/console-rest/wiki/using-the-js-library).

## Chrome Extension (Still in development)

Some API providers may have a Swagger/RAML/etc. but may not have included Console.REST as a Button in their API docs. Thanks to the awesome work of the guys at [apis.guru](https://apis.guru), the extension can offer the functionalities of Console.REST as a button even on pages that don't have the button.

## License

This repository is released under the [MIT License](LICENSE). Feel free to fork, and modify!
Copyright © 2016 Paw Inc.

## Contributors

See [Contributors](https://github.com/luckymarmot/console-rest/graphs/contributors).
