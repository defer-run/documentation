<p align="center">
    <picture>
        <source media="(prefers-color-scheme: dark)" srcset="https://www.defer.run/github/defer_darkmode.png" width="410" height="216">
        <img alt="Defer logo" src="https://www.defer.run/github/defer_lightmode.png" width="410" height="216">
    </picture>
</p>
<p>&nbsp;</p>
<p align="center">
    Zero infrastructure Node.js background jobs
</p>
<p>&nbsp;</p>
<p align="center">
    <a href="https://docs.defer.run/">Documentation</a>
    <span>&nbsp;·&nbsp;</span>
    <a href="https://www.defer.run/blog">Blog</a>
    <span>&nbsp;·&nbsp;</span>
    <a href="https://discord.gg/x2v84Vqsk6">Community</a>
    <span>&nbsp;·&nbsp;</span>
    <a href="https://github.com/defer-run/defer.client/discussions/categories/roadmap">Roadmap / RFCs</a>
</p>

<p>&nbsp;</p>
<p>&nbsp;</p>

# Documentation

This repository contains the `.mdx` source files along with the associated assets in `public/`.
The full Nextra app will be open-sourced later this year.

<br />

Did you spot a mistake or missing information?
Feel free to open a PR or a ticket ! - and respect our [Code of Conduct](./CODE_OF_CONDUCT.md).

<br />

## Reporting Security Issues

If you discover a security vulnerability in our open-source repositories or products, please get in touch with our security team immediately at security@defer.run. We appreciate
your responsible disclosure and will respond promptly to address the issue.

<br />

# Contributing

We welcome contributions!
The Defer documentation is built with [Nextra](https://nextra.site/) using [MDX files](https://mdxjs.com/); please follow the [Nextra documentation](https://nextra.site/docs/docs-theme/page-configuration) to add new pages and update the navigation.

<br />

Also, please find below the list of the components available in our documentation.

<br />
<br />

## Components

Our documentation uses some Nextra components: [`<Callout>`](https://nextra.site/docs/guide/built-ins), and [`<Tabs>/<Tab>`](https://nextra.site/docs/docs-theme/built-ins/tabs).

We also built our own, as listed below:

## `<Accordion>`

- [Live Demo](https://docs.defer.run/platform/setup-a-defer-application/)
- [Demo source](./pages//platform/setup-a-defer-application.mdx)

```mdx
import { Accordion } from "~components";

<Accordion title={'Set your Defer Token on Heroku'}>

...

</Accordion>

<Accordion title={'Set your Defer Token on AWS'}>

...

</Accordion>

<Accordion title={'Set your Defer Token on Vercel'}>

...

</Accordion>
```

<br />

## `mermaid` code

You can use the `mermaid` code block to display [mermaid](https://mermaid.js.org/syntax/flowchart.html) graphs.

- [Live Demo](https://docs.defer.run/features/cron)
- [Demo source](./pages/features/cron.mdx)

<br />

## `<Prerequisites>`

Used to display the knowledge or action prerequesites for the current page.

- [Live Demo](https://docs.defer.run/features/background-function)
- [Demo source](./pages/features/background-function)

<br />

The `items[].icon` values can be: `defer`, `key` or `layer` (ping us if you think a different icon is necessary).

```mdx
import { Prerequisites } from "~components";

### Prerequisites

<br />

<Prerequisites
  items={[
    {
      title: "Setup Defer",
      subtitle: "How to setup Defer with Next, Nest and more",
      icon: "layers",
      link: "/quickstart",
    },
  ]}
/>
```

<br />

## `<RepositoryCard>`

A nice way to link a GitHub repository.

<br />

- [Live Demo](https://docs.defer.run/features/local-development)
- [Demo source](./pages/features/local-development.mdx)

<br />

```mdx
import { RepositoryCard } from "~components";

<RepositoryCard
  name={"OpenAI + Next.js + Defer demo"}
  url={"https://github.com/defer-run/defer-openai-github-profile"}
/>
```
