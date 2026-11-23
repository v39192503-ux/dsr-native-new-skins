# Changelog — DSR Native 0.3.1 (Custom Skins)

## Atualização e créditos dos forks
- Base de atualização/compatibilidade: [fernanfez00/dsr-native-mali — Release 3.0](https://github.com/fernanfez00/dsr-native-mali/releases/tag/3.0), referência para a linha de melhorias voltadas à compatibilidade e suporte Mali.
- Base dos controles e assets de skin: [v39192503-ux/dsr-native-new-skins — v0.3.0](https://github.com/v39192503-ux/dsr-native-new-skins/releases/tag/v0.3.0). Esta versão mantém os assets e integra a renderização das skins ao overlay de controles.

## Novidades
- Integrados os assets de skin personalizados no TouchControls.
- Os 29 PNGs são carregados uma vez e mantidos em cache para reutilização na renderização.
- Visual personalizado para A/B/X/Y, L/R, ZL/ZR, Minus/Plus, direções do D-pad, L3 e Lock.
- Analógico esquerdo usa base e nub texturizados, com variantes de pressionado quando disponíveis.
- Variantes lit e overlay ring para feedback visual dos botões pressionados.
- Mantidos hitboxes, posição e lógica de toque, multitouch, arrasto de câmera e entrada de controle físico.
- O lado direito continua usando toque/arrasto de câmera; não foi introduzido analógico direito visual.

## Correções e build
- versionName 0.3.1 e versionCode 4 para atualizar sobre a versão anterior.
- CI usa GITHUB_RUN_NUMBER com valor mínimo 4.
- Build Android ARM64 com Gradle 8.7, SDK 34, NDK 26.1.10909125 e CMake 3.22.1.
- Testado instalando e abrindo no POCO F5; overlay de skin foi observado na tela de criação de personagem. Teste breve de abertura/renderização, não representa teste completo de gameplay.

## APK
- Package: com.dsrnative.app
- Version: 0.3.1 / versionCode 4
- ABI: arm64-v8a; Android 10+ (minSdk 29)
- APK debug; não é assinatura release de produção.
