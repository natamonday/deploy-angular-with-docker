# Deploy-Angular-with-Docker

### Descript : An example of how to deploy Angular appcalition with Docker.

***

<!-- ## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

 ## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io). 

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page. -->


### Init project
*install node modules with npm and yarn*
```console
npm install
```

### Run project
```console
npm start
```
### Build project
*build project generate dist*
```console
npm run build
```
### Run Unit testing
```console
npm run test
```
***
## :black_square_button: Container Image
### Build image
```console
docker build -f Dockerfile -t [NAME_IMAGE:TAG] .
```
*Example build image*
```console
docker build -f Dockerfile -t angular-app:v.1 .
```
### Run image as a container
```console
docker run -d -p [HOST_PORT]:[CONTAINER_PORT] --name [NAME_CONTRAINER] [NAME_IMAGE:TAG]
```

*Example run image as a container*
```console
docker run -d -p 4200:80 --name angular-app angular-app:v.1
```
