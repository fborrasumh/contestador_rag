# contestador_rag

App educativa de IA en un único fichero HTML, disponible como **aplicación web**
y como **ejecutable de escritorio** para Windows, macOS y Linux.

## 📥 Descargas (escritorio)

| Sistema | Fichero en [Releases](../../releases/latest) |
|---|---|
| 🪟 Windows 10/11 | `*_x64-setup.exe` (instalador) |
| 🍎 Mac Apple Silicon (M1–M4) | `*_aarch64.dmg` |
| 🍎 Mac Intel | `*_x64.dmg` |
| 🐧 Linux | `*.AppImage` (portable) o `*.deb` |

> ⚠️ **Primer arranque:** al no llevar firma comercial, el sistema mostrará un aviso.
> - **Windows:** *Más información → Ejecutar de todas formas*.
> - **macOS:** clic derecho sobre la app → *Abrir* → *Abrir*. Si persiste:
>   `xattr -cr /Applications/contestador_rag.app`
> - **Linux:** `chmod +x contestador-rag*.AppImage` y doble clic.

## 🔑 API keys

La app pide al usuario su propia api key (OpenAI / Anthropic / Google), que se
guarda solo en su equipo y únicamente viaja al servidor oficial del proveedor.

## 🛠️ Publicar una nueva versión

1. Edita `src/index.html`.
2. Sube la versión en `src-tauri/tauri.conf.json` y `src-tauri/Cargo.toml`.
3. `git commit` + `git push`.
4. `git tag vX.Y.Z && git push --tags` → los ejecutables aparecen en **Releases** (~15 min).
