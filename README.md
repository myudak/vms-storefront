## Vue js storefront medusa

## About

### Participants
myudak - @myudak

## Set up Project

### Prerequisites
Before you start with the tutorial make sure you have

- [Node.js](https://nodejs.org/en/) v14 or greater installed on your machine
- [VMS-medusa-admin](https://github.com/myudak/vmsMedusa-admin) run `npm install;npm start`
- [VMS-medusa-server](https://github.com/myudak/vmsMedusa-server) run `npm install;npm install -g @medusajs/medusa;medusa develop`
- [VMS-minIO](https://github.com/myudak/vmsMinIO) download [minIO](https://min.io/docs/minio/windows/index.html) place it in parent directory run `cd ..;./minio.exe server "path directory" --address :6900 --console-address :9090`

### Install Project

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

4. goto minIO page in `127.1.1:9090`:
![image](https://user-images.githubusercontent.com/69108782/194758258-2b41b42f-8b69-4ec3-96bf-30a022120064.png)

5. login with username and pass:
```bash
minioadmin
```
6. goto manage -> make accsess policy public
<br/>

![Untitled video - Made with Clipchamp](https://user-images.githubusercontent.com/69108782/194758492-d235dc80-043a-41f4-b758-371db7f28fef.gif)

<br>

7. goto identitiy -> service account -> create service account -> make the accsess key and the secret key :

```bash
ZfP0iiPrIndoL07v
```
```bash
Zetmnu1NVuJHeia887gJ8KeaRh6ULUaF
```

![Untitled video - Made with Clipchamp (1)](https://user-images.githubusercontent.com/69108782/194758995-d263cf1e-d124-499c-89a3-26f6007e4eb5.gif)

finish and see the web on 
```
http://localhost:8000/
```



