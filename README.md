# Base template Angular 15 + firebase 9.17.2 + authService (firebaseAuth) TESTING!!

Plantilla base con Angular 15 y Firebase, sin CSS, que incluye funcionalidades de inicio de sesión, cierre de sesión, control de acceso, registro de usuario y restablecimiento de contraseña. Además, agregué pruebas para las funciones del servicio de autenticación implementadas con Firebase.

Base template with Angular 15 and Firebase, without CSS, featuring login, logout, can activate, register, reset password functionalities. Additionally, I added testing for the authentication service functions implemented with Firebase.

# Primeros paso - First steps

Para utilizar este proyecto es necesario ejecutar el comando "npm install". Las versiones actuales que tengo instaladas son: Angular CLI 13.0.0, Node 14.15.4, Gestor de paquetes npm 6.14.10 y Firebase CLI 9.17.0.

To use this project, you need to run the "npm install" command. The current versions that I have installed are: Angular CLI 13.0.0, Node 14.15.4, Package Manager npm 6.14.10, and Firebase CLI 9.17.0.

# Project

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 15.1.2.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

# Setup notes

Es importante tener en cuenta que la biblioteca de Firebase puede generar errores en TypeScript, por lo que ya se ha agregado "skipLibCheck": true en el archivo tsconfig.json.

It's important to know that the Firebase library may cause errors in TypeScript, so "skipLibCheck": true has already been added to the tsconfig.json file.

# environments

Recuerda crear la carpeta "environments" dentro de "src" y asegúrate de incluir un archivo de configuración con tus datos de Firebase. El nombre del archivo debería ser algo como esto:

Remember to generate the "environments" folder within "src" and include a configuration file with your Firebase data. The filename should look something like this:

```
export const environment = {
  production: false,
  firebaseConfig: {
    apiKey: 'xxx',
    authDomain: 'xxx',
    projectId: 'xxx',
    storageBucket: 'xxx',
    messagingSenderId: 'xxx',
    appId: 'xxx',
    measurementId: 'xxx',
  },
};
```
