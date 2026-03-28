# Androidbin

Repositório de binários pré-compilados do Node.js para Android (aarch64/arm64).

## Como usar

Baixe o `node.zip` na aba [Releases](https://github.com/fernandosoon9-debug/Androidbin/releases).

### Estrutura do zip

```
node-android-aarch64/
  bin/node
  bin/npm
  bin/npx
  lib/node_modules/npm/
  include/node/
```

### URL para usar no ShellExecutor.java

```java
private static final String NODE_ZIP_URL =
    "https://github.com/fernandosoon9-debug/Androidbin/releases/download/NodeJS-v22.14.0-aarch64/node.zip";
```

## Build

O zip é gerado automaticamente via GitHub Actions usando:
- **Node.js v22.14.0**
- **Android NDK r26b**
- **API Level 24** (Android 7.0+)

Para gerar uma nova versão, vá em **Actions → Build Node.js v22 for Android aarch64 → Run workflow**.
