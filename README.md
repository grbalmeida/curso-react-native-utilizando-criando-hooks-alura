### Comando para iniciar o projeto

```
npx react-native init orgsHooks --version 0.65.1
```

### Comando para rodar o projeto

```
npx react-native start
```

```
npx react-native run-android
```

### Comando para gerar o APK utilizando a cli do React Native

Passo 1: Gerar o arquivo index.android.bundle

```
npx react-native bundle --platform android --dev false --entry-file index.js --bundle-output android/app/src/main/assets/index.android.bundle --assets-dest android/app/src/main/res
```

Passo 2: Acessar a pasta android

```
cd android
```

Passo 3: Dentro da pasta android rodar o comando abaixo:

```
gradlew assembleDebug
```

Arquivo será disponibilizado no path abaixo:

```
yourProject/android/app/build/outputs/apk/debug/app-debug.apk
```