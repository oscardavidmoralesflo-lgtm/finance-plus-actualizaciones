# Finance Plus · actualizaciones

Canal de actualizaciones de la app Android Finance Plus (`com.aurea.finance`).

Cada versión es un *release* `v<versión>` con dos archivos:

- `Finance-Plus-<versión>-Android.apk`
- `update.json` (`versionCode`, `versionName`, `apkName`, `sha256`, `notes`)

La app revisa `releases/latest/download/update.json` y, antes de instalar, comprueba que la versión sea más nueva, el SHA-256 del archivo y el certificado de firma (SHA-256 `feb96a39d3cc9bee9fcef7bda2247bf2a8e2685898dbf47bcbddc53a89378aed`).

Este repositorio no contiene datos personales ni código fuente.

## Publicar una versión

Copia la APK y su `update.json` en `entrega/` (borra la APK anterior) y haz push a `main`. El flujo `Publicar versión` comprueba el SHA-256 y crea el release.
