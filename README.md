<a href="https://chat.vercel.ai/">
  <img alt="Next.js 14 and App Router-ready AI chatbot." src="https://gemini-chatbot.vercel.rocks/og.png">
  <h1 align="center">Next.js AI Chatbot</h1>
</a>

<p align="center">
  An open-source AI chatbot app template built with Next.js, the Vercel AI SDK, Google Gemini, and Vercel KV.
</p>

<p align="center">
  <a href="#features"><strong>Features</strong></a> ·
  <a href="#model-providers"><strong>Model Providers</strong></a> ·
  <a href="#deploy-your-own"><strong>Deploy Your Own</strong></a> ·
  <a href="#running-locally"><strong>Running locally</strong></a> ·
  <a href="#authors"><strong>Authors</strong></a>
</p>
<br/>

## Features

- [Next.js](https://nextjs.org) App Router
- React Server Components (RSCs), Suspense, and Server Actions
- [Vercel AI SDK](https://sdk.vercel.ai/docs) for streaming chat UI
- Support for Google Gemini (default), OpenAI, Anthropic, Cohere, Hugging Face, or custom AI chat models and/or LangChain
- [shadcn/ui](https://ui.shadcn.com)
  - Styling with [Tailwind CSS](https://tailwindcss.com)
  - [Radix UI](https://radix-ui.com) for headless component primitives
  - Icons from [Phosphor Icons](https://phosphoricons.com)
- Chat History, rate limiting, and session storage with [Vercel KV](https://vercel.com/storage/kv)
- [NextAuth.js](https://github.com/nextauthjs/next-auth) for authentication

## Model Providers

This template ships with Google Gemini `models/gemini-1.0-pro-001` as the default. However, thanks to the [Vercel AI SDK](https://sdk.vercel.ai/docs), you can switch LLM providers to [OpenAI](https://openai.com), [Anthropic](https://anthropic.com), [Cohere](https://cohere.com/), [Hugging Face](https://huggingface.co), or using [LangChain](https://js.langchain.com) with just a few lines of code.

## Deploy Your Own

You can deploy your own version of the Next.js AI Chatbot to Vercel with one click:

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?demo-title=IAA+UFES&demo-description=Inteligencia+Artificial+Assistente+para+a+comunidade+Ufes%2C+usando+Next.js+e+a+API+de+Google+Gemini&demo-url=https%3A%2F%2Fiaa-ufes.vercel.app%2F&demo-image=https%3A%2F%2Fraw.githubusercontent.com%2Frenan-fa%2Fiaa_ufes%2Fmain%2Fpublic%2Fimages%2FIAA-UFES.png&project-name=IAA+UFES+Chatbot&repository-name=iaa_ufes&repository-url=https%3A%2F%2Fgithub.com%2Frenan-fa%2Fiaa_ufes&from=templates&skippable-integrations=1&env=GOOGLE_GENERATIVE_AI_API_KEY%2CAUTH_SECRET&envDescription=Como+obter+essas+vari%C3%A1veis+de+ambiente&envLink=https%3A%2F%2Fgithub.com%2Frenan-fa%2Fiaa_ufes%2Fblob%2Fmain%2F.env.example&teamCreateStatus=hidden&stores=%5B%7B%22type%22%3A%22kv%22%7D%5D)


## Running locally

You will need to use the environment variables [defined in `.env.example`](.env.example) to run Next.js AI Chatbot. It's recommended you use [Vercel Environment Variables](https://vercel.com/docs/projects/environment-variables) for this, but a `.env` file is all that is necessary.

> Note: You should not commit your `.env` file or it will expose secrets that will allow others to control access to your various Google Cloud and authentication provider accounts.

1. Install Vercel CLI: `npm i -g vercel`
2. Link local instance with Vercel and GitHub accounts (creates `.vercel` directory): `vercel link`
3. Download your environment variables: `vercel env pull`

```bash
pnpm install
pnpm dev
```

Your app template should now be running on [localhost:3000](http://localhost:3000/).

## Authors

This library is created by [Vercel](https://vercel.com) and [Next.js](https://nextjs.org) team members, with contributions from:

- Jared Palmer ([@jaredpalmer](https://twitter.com/jaredpalmer)) - [Vercel](https://vercel.com)
- Shu Ding ([@shuding\_](https://twitter.com/shuding_)) - [Vercel](https://vercel.com)
- shadcn ([@shadcn](https://twitter.com/shadcn)) - [Vercel](https://vercel.com)
- Jeremy Philemon ([@jrmyphlmn](https://twitter.com/jrmyphlmn)) - [Vercel](https://vercel.com)
