# **Deploy-Angular-with-Docker**

### Descript : An example of how to deploy Angular appcalition with Docker.

---

## :computer: **Development Project**
### **Init project**
*install node modules with npm and yarn*
```console
npm install
```
### **Run project**
```console
npm start
```
### **Unit testing**
```console
npm run test
```
### **Build Project**
*build project generate dist*
```console
npm run build
```
---
## :whale: **Deployment with Docker**
### **Image Registry**

> #### https://hub.docker.com/r/pramotser/angular-app

### **Build image**
```console
docker build -f Dockerfile -t [NAME_IMAGE:TAG] .
```
*Example build image*
```console
docker build -f Dockerfile -t angular-app:v.1 .
```
### **Run Image as a Container**
```console
docker run -d -p [HOST_PORT]:[CONTAINER_PORT] --name [NAME_CONTRAINER] [NAME_IMAGE:TAG]
```

*Example run image as a container*
```console
docker run -d -p 4200:80 --name angular-app angular-app:v.1
```

