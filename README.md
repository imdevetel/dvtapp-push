# dvtapp-push
Devetel IONIC App Push
```
git clone https://github.com/imdevetel/dvtapp-push.git  
npm install  
ionic cordova run android --verbose  
```
## Para configurar proxy:  

### Variables de Sistema:  
```
HTTP_PROXY = http://proxy.example.cl:8080  
HTTPS_PROXY = http://proxy.example.cl:8080  
IONIC_HTTP_PROXY = http://proxy.example.cl:8080  
```

### Gradle  
C:\Users\usuario\\.gradle (Buscar o crear archivo gradle.properties)  
```
systemProp.http.proxyHost=proxy.example.cl  
systemProp.http.proxyPort=8080  
systemProp.http.nonProxyHosts=localhost  
systemProp.https.proxyHost=proxy.example.cl  
systemProp.https.proxyPort=8080  
systemProp.https.nonProxyHosts=localhost  
```

### NPM  
```
npm config set proxy http://proxy.example.cl:8080  
npm config set https-proxy http://proxy.example.cl:8080  
```

### IONIC  
Global:  
```
npm install -g @ionic/cli-plugin-proxy  
```
Local proyect:  
```
cd myProject  
npm install --save-exact --save-dev @ionic/cli-plugin-proxy  
```

### GIT  
```
git config --global http.proxy http://proxy.example.com:8888  
```
