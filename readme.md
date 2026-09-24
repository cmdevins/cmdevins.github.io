# Time Travelers Pokemon League Website

## Setup

### Tools and System Dependencies

This project requires Node.js v24.12.0 and npm.

[nvm](https://github.com/nvm-sh/nvm) is highly recommended to manage both Node.js and npm installations. This project will assume you are using nvm. If not yet installed, follow the [installation steps for nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

#### Install System dependencies

The project's node version is saved in `.nvmrc`. nvm will read and use this version for the next steps.

Install the correct Node.js version for the project with the command:

```shell
nvm install
```

Then switch to your system Node.js version temporarily with the command:

```shell
nvm use
```

Optionally, verify the active Node.js version with the command:

```shell
node --version
```

It should print the same node version in `.nvmrc`.

Finally, follow the commands under [Development](#development) to verify everything is setup correctly.

## Development

Install project dependencies with npm. You will need to do this whenever `package.json` or `package-lock.json` is changed.

```shell
npm install
# or the shorthand
npm i
```

Run the local development server and open the URL it displays. The server will automatically refresh your browser page as files are saved.

```sh
npm run dev
```

## Build

To create a build of the static assets for the website, run the command:

```shell
npm run build
```

The build files will be put in `/dist`. These files can be served locally with the following command:

```shell
npm run preview
```

You can run the build and preview commands to verify all changes locally as they would appear in the deployed site. However, this is not significantly different than using the dev command.

## Deployment

Deployments are managed with Github Workflows and Actions. See [.github/workflows/deploy.yml](.github/workflows/deploy.yml).
