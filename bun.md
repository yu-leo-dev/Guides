# Bun 1.4

_13 Sep 2026_

> [!IMPORTANT]
> Если в системе установлен только Bun (без Node.js и npm), тогда лучше создать символьные ссылки, т.к. некоторые программы все еще требуют Node.js или npm.

```bash
ln -s $(which bun) $(dirname $(which bun))/node
ln -s $(which bun) $(dirname $(which bun))/npm
```

## 1. Build a React app with Bun

```bash
bun init my-bun-app --react
cd my-bun-app/
bun run build
```

> [!NOTE]
> 📦 Размер основного JS-бандла: 433 kB [client+server] (react-dom@19.3 210kB. А что остальное? Сервер?)
> 
> bun init my-bun-app --react=tailwind # 214 kB
> 
> bun init my-bun-app --react=shadcn # 349 kB

Ссылки

1. [Bun Site](https://bun.com/)
2. [Bun GitHub](https://github.com/oven-sh/bun) ⭐ 96k
3. [Bun в 2026](https://habr.com/ru/articles/1072980/)
4. 👉 [Build a React app with Bun](https://bun.com/guides/ecosystem/react)
