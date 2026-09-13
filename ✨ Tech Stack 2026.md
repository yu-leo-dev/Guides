# Технологический стек 2026 года

_12 Sep 2026_

[TypeScript 7.0](https://www.typescriptlang.org/) - язык программирования

Безоговорочный лидер. Один язык для всего. Сквозная типизация, начиная с базы данных и заканчивая фронтендом.

В перспективе можно еще посмотреть в сторону **Python, Go, Rust**

[Bun 1.4](bun.md) - среда выполнения Typescript

Предыдущее решение было **Node.js / npm / ts-node**. Несмотря на то, что Node.js пока [лидирует](https://2025.stateofjs.com/en-US/other-tools/#runtimes), а также научился самостоятельно выполнять TypeScript в последних версиях - поезд ушел. Bun уже на 3-м месте, опережая Deno.

⚠️ Для некоторых проектов Node все же еще нужен. Например для Strapi. Так что, его нужно пока установить параллельно с Bun. А вот npm и npx можно не устанавливать (либо удалить, если уже установлены). 

[React 19.3](https://react.dev/) - фронтенд фреймворк

Здесь даже думать нечего. Конкуренты Vue, Angular, Svelte - далеко [позади](https://2025.stateofjs.com/en-US/libraries/front-end-frameworks/)

[TanStack Start RC](tanstack-start.md), [Astro 7.3](https://astro.build/) - мета-фреймворки

Конечно же, почти все используют Next. На сегодня - это стандарт в отрасли. Но сложность Next и простота TanStack сделают свое дело. А серверные функции TanStack это вообще супер - можно писать фронтенд и бэкенд как одно целое. Никаких API. У Next и TanStack есть серверные компоненты, но это не то. TanStack также использует [Vite](vite.md), который вроде как лучше, чем Turbopack в Next.

React Router и Remix кажется проигрывают конкуренцию.

Astro - для контент-ориентированных сайтов

[Tailwind CSS 4.3](https://tailwindcss.com/) и [Shadcn/ui 4.21](shadcn-ui.md) - стилизация

Отраслевой стандарт. Особенно для ИИ.
Недавно появился Stylex + Astryx от Meta. Посмотрим.
Предыдущее решение - MUI. Однако MUI использует CSS-in-JS Emotion, что по нынешним временам плохо. Часть разработчиков MUI вообще занялась новым проектом Base UI, который стал дефолтным выбором в Shadcn/ui, наряду с Radix и React Aria.

[Strapi 5.52](https://strapi.io/) - CMS

[Elysia 1.4](https://elysiajs.com/) - бэкенд-фреймворк

Elysia выделяется тем, что является единственным, построенным на основе Bun. Использование совершенно новой среды выполнения может быть рискованным шагом, но, учитывая растущую популярность самого Bun, похоже, что эта ставка может оправдаться.
Ждем версию [2.0](https://elysiajs.com/blog/elysia-20.html)

Express устарел.

Также можно смотреть в сторону Fastify и Hono

[PostgreSQL 18.6](https://www.postgresql.org/), [Drizzle 0.45](https://orm.drizzle.team/) - база данных / ORM

PostgreSQL является основой практически любой разумной архитектуры. Он обрабатывает реляционные данные, JSON, полнотекстовый поиск и векторный поиск в одном движке.

Drizzle теперь является предпочтительным уровнем данных для многих команд по сравнению с Prisma, поскольку он обеспечивает лучшее определение типов TypeScript без сложного этапа генерации кода.

[BullMQ 6.3](https://bullmq.io/) с [Redis 8.10](https://github.com/redis/redis) - очередь заданий для фоновых задач

[Zod 4.5](https://zod.dev/) - валидация

[Apollo Server 5.5](https://www.apollographql.com/docs/apollo-server), [Apollo Client 4.2](https://www.apollographql.com/docs/react), [GraphQL Code Generator](https://the-guild.dev/graphql/codegen) - если нужен GraphQL API либо нормализованный кэш запросов

[Biome 2.5](https://biomejs.dev/) - линтер

Раньше была связка ESLint + Prettier.

Еще OXlint вроде ничего так.

[Sphinx 3.9](https://sphinxsearch.com/) - полнотекстовый поиск

Пока используем старый добрый Sphinx. Но, как-то он сильно устарел. Хотя Аксенов что-то еще пытается делать в Avito.
Нужно посмотреть в сторону встроенного поиска в PostgreSQL, а также RAG и т.п.

[VSCode 1.136](https://code.visualstudio.com/) - редактор кода

ИИ - ну куда же без него :)

Ссылки

1. [State of JavaScript 2025](https://2025.stateofjs.com/)
2. [State of JavaScript 2025-2026: Key Takeaways for Modern Web Development Teams](https://strapi.io/blog/state-of-javascript-2025-key-takeaways)
3. [The 2026 developer tech stack: what to learn, use, and skip](https://daily.dev/blog/developer-tech-stack-learn-use-skip/)
4. [The Complete Full-Stack Developer Roadmap for 2026](https://dev.to/thebitforge/the-complete-full-stack-developer-roadmap-for-2026-2i0j) - большая основательная статья
5. [The Best Web Development Stack in 2026 (And Why Most Developers Are Thinking About It Wrong)](https://medium.com/@sovannaro/the-best-web-development-stack-in-2026-and-why-most-developers-are-thinking-about-it-wrong-2d490a8445ed)
6. [React stack 2026: карта лучших библиотек по категориям](https://habr.com/ru/articles/1032830/)
