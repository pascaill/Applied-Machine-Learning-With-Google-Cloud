# Tampilan Aplikasi 
![Capturehome](https://raw.githubusercontent.com/pascaill/Deteksi-Kanker-Backend-API/master/Capturehome.PNG)
![Capturelol](https://raw.githubusercontent.com/pascaill/Deteksi-Kanker-Backend-API/master/Capturelol.PNG)

# Struktur Folder

```
src
├── exceptions
│   ├── ClientError.js
│   └── InputError.js
├── server
│   ├── handler.js
│   ├── routes.js
│   └── server.js
└── services
    ├── inferenceService.js
    ├── loadModel.js
    └── storeData.js
.env
DockerFile
package.json
credentials.json
README.md

```


# Cara Deploy

```
markdown

- Open Cloud Console
- git clone [This Repository]
- gcloud builds submit --tag gcr.io/[PROJECT ID]/[PROJECT DIRECTORY]
- gcloud run deploy backend-mlgc \
--image gcr.io/[PROJECT ID]/[PROJECT DIRECTORY] \
--set-env-vars APP_ENV=production,APP_PORT=8080,APP_HOST=0.0.0.0,MODEL_URL=[MODEL URL] \
--platform managed \
--region asia-southeast2 \
--allow-unauthenticated
  
```

# Deployed Backend 

