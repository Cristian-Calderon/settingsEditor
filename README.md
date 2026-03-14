# ⚙️ Editor Config

Configuración personal para VSCode y forks compatibles (Antigravity, Trae, Cursor, etc.).

## 📁 Estructura

```
editor-config/
├── README.md
├── settings.json         ← configuración completa del editor
└── VIM_SHORTCUTS.md      ← referencia rápida de todos los shortcuts de Vim
```

## 🛠️ Editores compatibles

Esta configuración funciona en cualquier editor basado en VSCode:

- **VSCode** — Microsoft
- **Antigravity** — fork de Google
- **Trae** — fork de ByteDance
- **Cursor** — fork con IA integrada
- **Windsurf** — fork de Codeium

## 🔌 Extensiones necesarias

Para que la config de Vim funcione al 100%:

- `vscodevim.vim` — Vim keybindings
- `esbenp.prettier-vscode` — formatter JS/TS/JSON
- `ritwickdey.LiveServer` — live server
- `Equinusocio.vsc-material-theme` — tema Material Ocean
- `PKief.material-icon-theme` — iconos

## 🚀 Cómo usar

1. Clona el repositorio
2. Copia `settings.json` en la carpeta de configuración de tu editor:
   - **VSCode/Antigravity/Trae** (Linux): `~/.config/Code/User/settings.json`
   - **VSCode** (macOS): `~/Library/Application Support/Code/User/settings.json`
3. Instala las extensiones listadas arriba
4. Consulta `VIM_SHORTCUTS.md` para ver todos los atajos disponibles
