<h1 align="center">
  VMS Storefront
</h1>

<div style="display:flex;justify-content:center;align-items:center">
<div>
    <img alt="Plus" style="margin-right:18px" src="https://user-images.githubusercontent.com/75976169/197110145-a10e636f-ba10-4bed-aa45-83ff41222159.png" width="63" />
</div>

<div>
    <img alt="Plus" src="https://user-images.githubusercontent.com/75976169/197108692-5048d15b-1b8d-4bf8-ab3f-83d9db689580.png" width="40" />
</div>

<a href="https://www.medusa-commerce.com">
    <img alt="Medusa" src="https://user-images.githubusercontent.com/7554214/153162406-bf8fd16f-aa98-4604-b87b-e13ab4baf604.png" width="100" />
</a>
</div>

<p align="center">A storefront built using <strong>MedusaJS</strong> +  <strong>VueJS</strong></p>

### Preview

![screencapture-localhost-8000-2022-10-09-17_19_05](https://user-images.githubusercontent.com/75976169/197107600-2e1da733-7ee2-4310-a131-475489cef7e0.png)

## About

### Participants

myudak - [@myudak](https://github.com/myudak)

Rohit Tewari - [@rtewari056](https://github.com/rtewari056)

## Set up Project

### Prerequisites
Before you start with the tutorial make sure you have:

- [Node.js](https://nodejs.org/en/) v14 or greater installed on your machine
- [VMS-medusa-admin](https://github.com/myudak/vmsMedusa-admin) run `npm install;npm start`
- [VMS-medusa-server](https://github.com/myudak/vmsMedusa-server) run `npm install;npm install medusa-file-minio;npm install -g @medusajs/medusa;medusa develop`
- [VMS-minIO](https://github.com/myudak/vmsMinIO) download [minIO](https://min.io/docs/minio/windows/index.html) place it in parent directory run `cd ..;./minio.exe server "path directory" --address :6900 --console-address :9090`

### Install Project

Done with the pre-requisites?

Here are the steps to be taken after that :

1. Clone the repository:
```bash
git clone https://github.com/myudak/vms-storefront
```

2. Change directory and install dependencies:
```bash
cd vms-storefront
npm install
```
3.  Start the app
```bash
npm run dev
```

4. Go to minIO page in `127.1.1:9090`:

![image](https://user-images.githubusercontent.com/69108782/194758258-2b41b42f-8b69-4ec3-96bf-30a022120064.png)

5. Login with username and password:
```bash
minioadmin
```
6. Go to manage -> make accsess policy public
<br/>

![Untitled video - Made with Clipchamp](https://user-images.githubusercontent.com/69108782/194758492-d235dc80-043a-41f4-b758-371db7f28fef.gif)

<br>

7. Go to identitiy -> service account -> create service account -> make the accsess key and the secret key :

```bash
ZfP0iiPrIndoL07v
```
```bash
Zetmnu1NVuJHeia887gJ8KeaRh6ULUaF
```

![Untitled video - Made with Clipchamp (1)](https://user-images.githubusercontent.com/69108782/194758995-d263cf1e-d124-499c-89a3-26f6007e4eb5.gif)

Finish and see the web on :
```
http://localhost:8000/
```



