<h1 align="center">
  <br>
  <a href="https://github.com/mithusingh32/ulralight-svelte-boilerplate#readme"><img src="https://i.imgur.com/6XvnLFJ.png" alt="header" width="600"/></a>
  <br>
  Ultralight Svelte Starter
  <br>
</h1>

Build desktop applications using a smaller, lighter, cross-platform WebKit that's more customizable and designed to display web technologies like Svelte. This is an [Ultralight](https://github.com/ultralight-ux/Ultralight) starter with [Svelte](https://svelte.dev/) with TypeScript. 


<p align="center">
  <img src="https://i.imgur.com/0iLU6L7.png" alt="ultralight" width="600"/>
</p>

## Available Commands


### Svelte
Commands you can execute inside the [Svelte](https://svelte.dev/) `app` directory

| Command | Description |
|---------|-------------|
| `yarn install` | Install project dependencies |
| `yarn build` | Builds code bundle with production settings  |
| `yarn dev` | Run a web server to serve built code bundle |

### Ultralight
Commands you can execute inside the build 

| Command | Description |
|---------|-------------|
| `cmake --build . --config Release` | Build Ultralight binary without cleaning |
| `cmake --build . --config Release --clean-first` | Build Ultralight binary |

## Prerequisites

Before you build and run, you'll need to [install the Ultralight prerequisites](https://docs.ultralig.ht/docs/installing-prerequisites) for your platform.

You also need to [install NodeJS](https://nodejs.org/en/download/) to work with Svelte
## Development

### Svelte

Inside the `app` folder resides Svelte, you need to install dependencies by executing the following commands

```shell
yarn
```

Before anything else you need to build the Svelte project. You need to do this everytime you want to test the desktop application.

```shell
yarn build
```

### Ultralight

Setup the Ultralight build folder, you only have to do this once by executing the following commands

```shell
mkdir build
cd build
cmake ..
cmake --build . --config Release
```

Once the above is setup everytime you need to rebuild the application you need to execute the following on the `build` directory

```shell
cmake --build . --config Release --clean-first
```

> Note you may need to delete the binary eg. `MyApp` in this case.


## Running

### Ultralight 
#### On macOS and Linux

Navigate to `ultralight-quick-start/build` and run `MyApp` to launch the program.

#### On Windows

Navigate to `ultralight-quick-start/build/Release` and run `MyApp` to launch the program.

### Svelte

To run your Svelte application and debug, just go to `app` folder and execute the
```shell
yarn dev
```

## Further Reading

Follow the [Writing Your First Ultralight App](https://docs.ultralig.ht/docs/writing-your-first-app) guide and other tutorials in the documentation for more info.

The Svelte application is created with [Svelte Template](https://svelte.dev/)

## Contributions
Huge thank you to [geocine](https://github.com/geocine/) for the idea. 

This project is based on [Ultralight-React Template](https://github.com/geocine/ultralight-react) Ultralight-React boilerplate. 