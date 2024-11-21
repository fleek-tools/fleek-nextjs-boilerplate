# Fleek Next.js Boilerplate

This is the boilerplate code generated directly from running `npx create-next-app`. Utilize this template to harness [Fleek’s](https://fleek.xyz/) optimized hosting for dynamic and performance-driven web applications

## Prerequisites

- Node 18.18.0+
- Fleek Account
- [Fleek CLI](https://fleek.xyz/docs/cli/)
- [Fleek Next Adapter](https://www.npmjs.com/package/@fleek-platform/next)

## Getting Started

1. Fork the repository
2. Clone the repository by running the following command:

```bash
git clone <https://github.com/><your-id>/fleek-nextjs-boilerplate.git
```

3. Enter the correct directory, install dependencies, and run locally:

```bash
cd fleek-nextjs-boilerplate
npm i
npm run dev
```

4. Ensure that you install the Fleek CLI and the Fleek Next Adapter:

```bash
// local installation
npm i @fleek-platform/cli
npm i @fleek-platform/next

// global installation
npm i -g @fleek-platform/cli
npm i -g @fleek-platform/next

```

> [!NOTE]
> You can check the Fleek CLI version by running `fleek -v`.
> Any version >= `2.10.1` should be good.
>
> As for the Fleek Next adapter, you can check the Fleek Next Adapter version by running `fleek-next -v`.
> Any version >= `2.1.0` should be good.

## Building and Deploying

### 1. Build the project

Build the project using the Fleek Next Adapter:

```bash
npx fleek-next build
# or if installed globally
fleek-next build
```

### 2. Fleek Function

Now, Create the Fleek Function using the Fleek CLI:

```bash
//syntax
fleek functions create --name '<name of your function>'

//example
fleek functions create --name nextra-function

```

### 3. Deploy

Finally, deploy using the Fleek CLI:

```bash
//syntax
fleek functions deploy --bundle=false --path .fleek/dist/index.js --assets .fleek/static --name '<name of your function>'

//example
fleek functions deploy --bundle=false --path .fleek/dist/index.js --assets .fleek/static --name nextra-function
```

As you complete all the steps successfully here, you will be able to access your fullstack Next.js app using a link that looks like this- https://brief-disease-harsh.functions.on-fleek.app/

## Contributing

### Reporting Issues

- Use GitHub Issues to report bugs or suggest features.
- Provide clear details and steps to reproduce any issues.

### Pull Requests

- Fork the repository.
- Create a feature branch:

```bash
git checkout -b feature/your-feature
```

- Commit changes with clear messages.
- Push to your fork and submit a pull request.

## Learn More

- [Other Next.js templates](https://app.fleek.xyz/templates/)
- [Fleek CLI Docs](https://fleek.xyz/docs/cli/)
- [Fleek Function Docs](https://fleek.xyz/docs/cli/functions/)
- [Fleek Next Docs](https://fleek.xyz/docs/cli/fleek-next-adapter/)
- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.
