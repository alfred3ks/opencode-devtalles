### OpenCode instalacion.

Vamos a instalar OpenCode CLI, tenemos en enlace de su web.

https://opencode.ai/

Vamos a hacer la instalacion usando curl, abrimos la terminal de windows y ejecutamos: OJO esa terminal ya la tenemos configurada para ejecutar comandos de bash

```bash
curl -fsSL https://opencode.ai/v2/install | bash
```

Para ver la version que esta corriendo:

```bash
opencode --version
```

Si tratamos de correr opencode en la terminal bash de vscode y sale este fallo:

```bash
$ opencode
NVM blocked package-manager execution because a delegated command could not be trusted.

Command: opencode
File: C:\Users\alfsa\AppData\Local\Author Software\nvm\installs\v22.12.0\opencode.cmd
Reason: delegated script changed since it was trusted
Action: Reinstall this Node.js version or run `nvm reshim` after a trusted install.
If this change was unexpected, contact your administrator and review NVM event logs.
Event code: NVM4306
```

Bastara con ejecutar:

```bash
nvm reshim
```

Sirve para recrear/actualizar los enlaces (shims) que NVM usa para localizar los comandos instalados globalmente con Node.js.

Seguimos...
