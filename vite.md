# Vite 8.3

_13 Sep 2026_

## 1. Getting Started

```bash
bun create vite my-vite-app # React, TypeScript, Oxlint, install with Bun - no
cd my-vite-app
bun i
bun run build
```
**package.json**
```json
  "scripts": {
    "dev": "bunx --bun vite",
    "build": "tsc -b && bunx --bun vite build",
  },
```

> [!NOTE]
> 📦 Размер основного JS-бандла: 223 kB
>
> Особенности: Oxlint

> [!NOTE]
> Интересно, что Bun вместо связки Vite+Bub [предлагает перейти](https://bun.com/guides/ecosystem/vite) на [импорт HTML](https://bun.com/docs/bundler/fullstack) 

Ссылки

1. [Vite Site](https://vite.dev/)
2. [Vite GitHub](https://github.com/vitejs/vite) ⭐ 82.8k
3. 👉 [Scaffolding Your First Vite Project](https://vite.dev/guide/#scaffolding-your-first-vite-project)
4. [Build a frontend using Vite and Bun](https://bun.com/guides/ecosystem/vite)
