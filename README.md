# Carlton's Tools GUI

## Creation History

Followed Taui set before running commands below.

- https://tauri.app/start/prerequisites/

```bash
npm create tauri-app@latest
cd ccajtoolsgui
npm i
npm run tauri dev
WEBKIT_DISABLE_DMABUF_RENDERER=1 npm run tauri dev
```

```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
# need to do some vite setup before running this command
npx shadcn@latest init -d
npm i -D @types/node
npx shadcn@latest add button
```

## Bug Fix

Use
`ccajtoolsgui WEBKIT_DISABLE_DMABUF_RENDERER=1 npm run tauri dev`
to fix the following error
`AcceleratedSurfaceDMABuf was unable to construct a complete framebuffer`
which solves the blank window opening.