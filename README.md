# Comedy Connector

Comedy Connector is the open-source project that allows a city's comedy community to connect, especially up-and-coming
talent.

## Features

TODO

## Demo

TODO

## Steps used to create this project

- [x] Initialize workspace

  ```bash
  ng new comedy-connector --strict --create-application=false \                                                       ─╯
     --new-project-root=libs \
     --package-manager=pnpm
  pnpm install @schematics/angular@latest
  ng add @schematics/angular
  ng add @angular-eslint/schematics # add eslint schematics
  ```

- [x] Update Angular version to latest

  ```bash
  ng update @angular/cli @angular/core
  ```

- [x] Enable strict template type checking

  ```bash
  npm install --save-dev json
  npx json -I -f tsconfig.json -e "delete this.angularCompilerOptions.fullTemplateTypeCheck"
  npx json -I -f tsconfig.json -e "this.angularCompilerOptions.strictTemplates = true"
  ```

- [x] Generate the frontend application

  ```bash
  ng generate @angular-eslint/schematics:application cc-frontend --prefix=cc \
    --project-root=apps/frontend/cc-frontend \
    --style=scss --routing=true
  ng serve cc-frontend # verify
  ```

- [ ] Connect to Amplify

  ```bash
  code
  ```

- [ ] Setup additional targets: lint and e2e testing

  ```bash
  ng lint cc-frontend
  ng e2e cc-frontend
  ```

---

- [x] Task

  ```bash
  code
  ```

---

- [x] Setup e2e tests with WebDriverIO

  ```bash
  ng e2e 
  ```

---

- [x] Setup Amplify CLI - [see docs](https://docs.amplify.aws/angular/start/getting-started/installation/#configure-the-amplify-cli)
- [x] Add polyfill - [see docs](https://docs.amplify.aws/angular/start/project-setup/create-application/)
- [x] Create libs
  - nx generate @nx/angular:library appsync  --unitTestRunner=jest --style=scss --tags=shared --directory=libs/appsync
- [ ] Create Amplify backend - steps adapted from this [nx angular amplify tutorial](https://dev.to/beavearony/getting-started-with-a-angularnx-workspace-backed-by-an-aws-amplify-graphql-api---part-1-24m0)
  - Generate the angular library: `nx generate @nx/angular:library appsync`
  -
  - NOTE: the [amplify docs to create an app](https://docs.amplify.aws/angular/start/project-setup/create-application/) do not work with the nx setup
- [x] Setup Amplify UI components - [see docs](https://ui.docs.amplify.aws/angular/getting-started/installation)
- Setup additional Angular features from [Amplify Dev Center](https://docs.amplify.aws/angular/)
  - [ ] Pre-built UI components
  - [ ] Auth
  - [ ] Serverless backend
  - [ ] Storage
  - [ ] GraphQL
- [ ] [Setup CI](https://nx.dev/recipes/ci)

## Tech Stack

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 17.1.1.

- [Angular](https://angular.io) – framework
- [Typescript](https://www.typescriptlang.org/) – language
- [AWS Amplify](https://aws.amazon.com/amplify/) - Deployment Framework
- [nx](https://nx.dev/getting-started/intro) - Build system - ✨ **This workspace has been generated by [Nx, Smart Monorepos · Fast CI.](https://nx.dev)** ✨

## Getting Started

1. Prerequisites. Here's what you need to be able to run Comedy Connector locally:

   - Node.js
   - npm
   - npm global installs: `npx` `@angular/cli` `pnpm` `nx`

2. Clone the repository

3. Build: `pnpm install'

4. Run the dev server: `pnpm run serve`  

5. Visit [http://localhost:4200/](http://localhost:4200/) in your browser. The application will automatically reload
    if you change any of the source files.

## Development

### Start the app

To start the development server run `pnpm run serve`. Open your browser and navigate to <http://localhost:4200/>

### Running unit tests

`nx test <app>` or to run all tests `pnpm run test`

### Running end-to-end tests

`nx e2e frontend` or to run all tests `pnpm run e2e`

### Running tasks

- To execute tasks with Nx use the following syntax: `nx <target> <project> <...options>`
- You can also run multiple targets: `nx run-many -t <target1> <target2>`
- ..or add `-p` to filter specific projects: `nx run-many -t <target1> <target2> -p <proj1> <proj2>`
- Targets can be defined in the `package.json` or `projects.json`. Learn more [in the docs](https://nx.dev/features/run-tasks).

### Affected changes

- See what's been affected by changes: `nx affected:graph`
- run tests for current changes: `nx affected:test`
- run e2e tests for current changes: `nx affected:e2e`

### Editor Integration

Have a look at the [Nx Console extensions](https://nx.dev/nx-console). It provides autocomplete support, a UI for exploring and running tasks & generators, and more! Available for VSCode, IntelliJ and comes with a LSP for Vim users.

### Generate code

If you happen to use Nx plugins, you can leverage code generators that might come with it.

Run `nx list` to get a list of available plugins and whether they have generators. Then run `nx list <plugin-name>` to see what generators are available.

Learn more about [Nx generators on the docs](https://nx.dev/features/generate-code).

## Ready to deploy?

Just run `nx build comedy-connector` to build the application. The build artifacts will be stored in the `dist/` directory, ready to be deployed.

## Further help

See [nx docs](https://nx.dev/getting-started/intro)

## Contributing

Comedy Connector is an open-source project and we welcome contributions from the community.

If you'd like to contribute, please fork the repository and make changes as you'd like. Pull requests are welcome.

### Our Contributors ✨

<a href="https://github.com/RainyMrGab/comedy-connector/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=RainyMrGab/comedy-connector" />
</a>

## Resources

- [How to set up an Nx-style monorepo workspace with the Angular CLI](https://dev.to/this-is-angular/how-to-set-up-an-nx-style-monorepo-workspace-with-the-angular-cli-part-1-16b5)

## Inspiration

- [improvcoaches](https://github.com/JoeMcB/improvcoaches)
- [How to write a perfect README](https://dev.to/mfts/how-to-write-a-perfect-readme-for-your-github-project-59f2)
