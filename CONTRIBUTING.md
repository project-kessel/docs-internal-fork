# Contributing

## 🚀 Project Structure

Inside of your Astro + Starlight project, you'll see the following folders and files:

```
.
├── public/
├── src/
│   ├── assets/
│   ├── content/
│   │   ├── docs/
│   │   └── config.ts
│   └── env.d.ts
├── astro.config.mjs
├── package.json
├── tailwind.config.mjs
└── tsconfig.json
```

Starlight looks for `.md` or `.mdx` files in the `src/content/docs/` directory. Each file is exposed as a route based on its file name.

Images can be added to `src/assets/` and embedded in Markdown with a relative link.

Static assets, like favicons, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command             | Action                                           |
| :------------------ | :----------------------------------------------- |
| `npm install`       | Installs dependencies                            |
| `npm run dev`       | Starts local dev server at `localhost:4321`      |
| `npm run build`     | Build your production site to `./dist/`          |
| `npm run preview`   | Preview your build locally, before deploying     |
| `npm run astro ...` | Run CLI commands like `astro add`, `astro check` |

## Writing documentation

See [Writing documentation](src/content/docs/contributing/documentation.mdx).

## Internal documentation

This repository can be forked to augment with internal deployment documentation. [config-overlay.mjs](config-overlay.mjs) is designed to be overridden by forks in order to modify the sidebar for the inclusion of e.g. internal documentation.

Keep this in mind when making changes to this repository–note which repository you are working in. Inside the fork, you MUST not modify files which come from the public docs repository. In the public docs repository, care must be taken when modifying explicitly shared and overriden files, like `config-overlay.mjs`.
