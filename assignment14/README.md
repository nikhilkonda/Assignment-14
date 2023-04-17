I have used Loopback tool to do this assignment wherein I used the following commands 
Install node.js
$ npm install -g @loopback/cli
$ lb4 app
and I have clicked enter as per the instructions given
$ cd getting-started
$ npm start
Used  $ lb4 controller to add Controller to the code 
[?] Controller class name: hello
[?] What kind of controller would you like to generate? Empty Controller
    create src/controllers/hello.controller.ts
    update src/controllers/index.ts
Controller Hello was now created in src/controllers/
import {get} from '@loopback/rest';
export class HelloController {
  @get('/hello')
  hello(): string {
    return 'Hello world!';
  }
}
and I visited Visit http://127.0.0.1:3000/hello to see the desired output Hello world!



# assignment14

This application is generated using [LoopBack 4 CLI](https://loopback.io/doc/en/lb4/Command-line-interface.html) with the
[initial project layout](https://loopback.io/doc/en/lb4/Loopback-application-layout.html).

## Install dependencies

By default, dependencies were installed when this application was generated.
Whenever dependencies in `package.json` are changed, run the following command:

```sh
npm install
```

To only install resolved dependencies in `package-lock.json`:

```sh
npm ci
```

## Run the application

```sh
npm start
```

You can also run `node .` to skip the build step.

Open http://127.0.0.1:3000 in your browser.

## Rebuild the project

To incrementally build the project:

```sh
npm run build
```

To force a full build by cleaning up cached artifacts:

```sh
npm run rebuild
```

## Fix code style and formatting issues

```sh
npm run lint
```

To automatically fix such issues:

```sh
npm run lint:fix
```

## Other useful commands

- `npm run migrate`: Migrate database schemas for models
- `npm run openapi-spec`: Generate OpenAPI spec into a file
- `npm run docker:build`: Build a Docker image for this application
- `npm run docker:run`: Run this application inside a Docker container

## Tests

```sh
npm test
```

## What's next

Please check out [LoopBack 4 documentation](https://loopback.io/doc/en/lb4/) to
understand how you can continue to add features to this application.

[![LoopBack](https://github.com/loopbackio/loopback-next/raw/master/docs/site/imgs/branding/Powered-by-LoopBack-Badge-(blue)-@2x.png)](http://loopback.io/)
