# Shadcn with Turborepo

![Static Badge](https://img.shields.io/badge/shadcn%2Fui-2.0.5-blue?link=https%3A%2F%2Fgithub.com%2Fshadcn%2Fui)

This is a Turborepo demo repository with shadcn, tailwind, eslint, and typescript pre-configured.

> [!NOTE]
> This example uses `yarn` as a package manager.

## Using this example

Clone the repository:

```sh
git clone https://github.com/suyash5053/shadcn-turborepo.git
```

Install dependencies:

```sh
cd shadcn-turborepo
yarn install
```

### Add UI components

There are two ways:

1. Change your directory into the package and use
```sh
cd packages/ui
npx shadcn@latest add <component-name>
```
2. Adding via the `workspace` command.

> [!NOTE]
> Remember to run `yarn install` after copying an app.

### Utilities

This Turborepo has some additional tools already set for you:

- [TypeScript](https://www.typescriptlang.org/) for static type checking
- [ESLint](https://eslint.org/) for code linting
- [TailwindCSS](https://tailwindcss.com/) for better styling

### Build

To build all apps and packages, run the following command:

```sh
cd shadcn-turborepo
yarn build
```

### Develop

To develop all apps and packages, run the following command:

```sh
cd shadcn-turborepo
yarn dev
```

### Remote Caching

Turborepo can use a technique known as [Remote Caching](https://turbo.build/repo/docs/core-concepts/remote-caching) to share cache artifacts across machines, enabling you to share build caches with your team and CI/CD pipelines.

By default, Turborepo will cache locally. To enable Remote Caching you will need an account with Vercel. If you don't have an account you can [create one](https://vercel.com/signup), then enter the following commands:

```
cd shadcn-turborepo
npx turbo login
```

This will authenticate the Turborepo CLI with your [Vercel account](https://vercel.com/docs/concepts/personal-accounts/overview).

Next, you can link your Turborepo to your Remote Cache by running the following command from the root of your Turborepo:

```sh
npx turbo link
```

## Useful Links

Learn more about the power of Turborepo:

- [Tasks](https://turbo.build/repo/docs/core-concepts/monorepos/running-tasks)
- [Caching](https://turbo.build/repo/docs/core-concepts/caching)
- [Remote Caching](https://turbo.build/repo/docs/core-concepts/remote-caching)
- [Filtering](https://turbo.build/repo/docs/core-concepts/monorepos/filtering)
- [Configuration Options](https://turbo.build/repo/docs/reference/configuration)
- [CLI Usage](https://turbo.build/repo/docs/reference/command-line-reference)

Learn more about shadcn/ui:

- [Documentation](https://ui.shadcn.com/docs)
