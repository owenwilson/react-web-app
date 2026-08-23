# react web app

- In this example, I"m using pnpm because I saw many reports of supply chain attacks on npm, so now we're using pnpm to have better control and security.

## setup
 
- create proyect react

```sh
pnpm create next-app
✔ What is your project named? … react-web-app
✔ Would you like to use the recommended Next.js defaults? › No, customize settings
✔ Would you like to use TypeScript? … No / Yes
✔ Which linter would you like to use? › ESLint
✔ Would you like to use React Compiler? … No / Yes
✔ Would you like to use Tailwind CSS? … No / Yes
✔ Would you like your code inside a `src/` directory? … No / Yes
✔ Would you like to use App Router? (recommended) … No / Yes
✔ Would you like to customize the import alias (`@/*` by default)? … No / Yes
✔ What import alias would you like configured? … @/*
✔ Would you like to include AGENTS.md to guide coding agents to write up-to-date Next.js code? … No / Yes
Creating a new Next.js app in /home/user/react-web-app.
```

## scan vulnerabilities

- [clamav scan tool](https://www.clamav.net/)

```sh
clamscan -v -i -r ./react-web-app
```

- [trivy scan tool](https://github.com/owenwilson/trivy-scanner)

```sh
docker exec -it trivy-scanner trivy fs /root/react-web-app
```

```sh
docker exec -it trivy-scanner trivy --severity HIGH fs /root/react-web-app
```

## Getting Started
 
First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## references

- check out [official documentation react]()
- check out [inside keyv npm compromise preinstall malware trusted provenance ide hooks](https://snyk.io/blog/inside-keyv-npm-compromise-preinstall-malware-trusted-provenance-ide-hooks/)
- check out [chaindrop supply chain compromise anatomy self propagating worm](https://www.microsoft.com/en-us/security/blog/2026/08/04/chaindrop-supply-chain-compromise-anatomy-self-propagating-worm/)
 
