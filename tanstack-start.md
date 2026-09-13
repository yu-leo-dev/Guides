# TanStack Start RC

_13 Sep 2026_

## 1. Getting Started

```bash
bunx @tanstack/cli create my-tanstack-app
```

Выбираем React, Biome, Nitro, demo/examples - No.
В add-ons пока ничего не выбираем (позже попробовать Strapi, Compiler, Drizzle, Shadcn, T3Env, Apollo Client, Tanstack Query).
Git - No.

⚠️ Agent skills: yes; TanStack Intent configured

⚠️ Command "bunx --bun @tanstack/intent install" did not run successfully. Please run this manually in your project.

Как все это отключить? Ответ: --no-intent

```bash
cd my-tanstack-app
bun run build
bun preview
```

Ok. Запускается. Работает.

ℹ️ Чтобы не было ошибок гидрации в консоли Chrome, желательно максимально отключить расширения в Chrome.

📦 Размер основного JS-бандла: 342kB

⚠️ Почему-то нет файла favicon.ico (в прошлых версиях, вроде, был).

⚠️ Nitro 3 все еще в стадии beta.

### Попробуем абсолютно минимальный проект

```bash
bunx @tanstack/cli create my-tanstack-app --blank --no-git --yes
```
Все то же самое, только нет Nitro (билдится не в папку ./output, а в ./dist). Нет Tailwind и DevTools.

### Examples

Можно выбрать примеры.

**Events** - появились коллекции и документы, а также AI assistant. Интересно. Позже изучить

```
Starting content-collections with config content-collections.ts
... finished build of 2 collections and 14 documents in 491ms
```

Добавились: @tanstack/ai-...

❗📦 Размер основного JS-бандла: 499 kB + еще много чанков

**Resume**

Добавились: shadcn/ui (Radix), @tanstack/ai-...

❗📦 Размер основного JS-бандла: 1015 kB + чанк routes 103 kB

### Моя итоговая конфигурация

```bash
bunx @tanstack/cli create my-tanstack-app --yes --toolchain biome --deployment nitro --no-intent

```
📦 Размер основного JS-бандла: 350 kB (Добавилось demo. Всего 8 запросов, 502 kB. Из них 2 шрифта Fraunces суммарно около 90 kB). Demo - в принципе, нормально. Готовый Layout, переключатель dark/light.

Ссылки

1. [TanStack Start Site](https://tanstack.com/start/latest)
2. 👉 [Getting Started](https://tanstack.com/start/latest/docs/framework/react/getting-started)
3. [Use TanStack Start with Bun](https://bun.com/guides/ecosystem/tanstack-start) - Hosting
