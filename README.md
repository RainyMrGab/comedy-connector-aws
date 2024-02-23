# Comedy Connector

Comedy Connector is the open-source project that allows a city's comedy community to connect, especially up-and-coming
talent.

## Features

TODO

## Demo

TODO

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
   - npm global installs: `npx` `@angular/cli` `pnpm` `nx` TODO

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

## Amplify

`amplify status` will show you what you've added already and if it's locally configured or deployed
`amplify add <category>` will allow you to add features like user login or a backend API
`amplify push` will build all your local backend resources and provision it in the cloud
`amplify console` to open the Amplify Console and view your project status
`amplify publish` will build all your local backend and frontend resources (if you have hosting category added) and provision it in the cloud

## Contributing

Comedy Connector is an open-source project and we welcome contributions from the community.

If you'd like to contribute, please fork the repository and make changes as you'd like. Pull requests are welcome.

### Contributors ✨

<a href="https://github.com/RainyMrGab/comedy-connector/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=RainyMrGab/comedy-connector" />
</a>

## Resources

- TODO docs
- [How to set up an Nx-style monorepo workspace with the Angular CLI](https://dev.to/this-is-angular/how-to-set-up-an-nx-style-monorepo-workspace-with-the-angular-cli-part-1-16b5)

## Inspiration

- [improvcoaches](https://github.com/JoeMcB/improvcoaches)
- [How to write a perfect README](https://dev.to/mfts/how-to-write-a-perfect-readme-for-your-github-project-59f2)
