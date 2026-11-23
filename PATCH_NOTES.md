# DSR Native — correções do fork para APK 0.3.1

## O que foi alterado
- O versionCode local passou para 4 e o versionName para 0.3.1, permitindo atualizar a instalação 0.3.0 (versionCode 3).
- Builds de CI usam GITHUB_RUN_NUMBER com piso 4.
- Mantida assinatura debug fixa do fork (SHA-256: 53a1a386520c4e2bfedc703974d8864877277a9d2ff10700ef1c8284cbc4101f), compatível com o APK v0.3.0-skins.
- Restaurados os assets do APK v0.3.0-skins: 29 PNGs de skin, NOTICE e pacote Turnip (31 assets no total).
- Compilação Android ARM64 concluída no Windows com Gradle 8.7, SDK 34, NDK 26.1.10909125 e CMake 3.22.1.

## APK
- Pacote: com.dsrnative.app
- Versão: 0.3.1
- versionCode: 4
- ABI: arm64-v8a
- minSdk: 29 (Android 10+)
- Debug APK, não release signed.

## Build local
```powershell
cd android
gradle assembleDebug --no-daemon
```
