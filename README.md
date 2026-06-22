# Medium Clone 📝

> A full-featured blogging platform built with Next.js 14 and Sanity CMS — inspired by Medium.

![Next.js](https://img.shields.io/badge/Next.js-14-000000?style=flat-square&logo=next.js)
![Sanity](https://img.shields.io/badge/Sanity-CMS-F03E2F?style=flat-square&logo=sanity)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=flat-square&logo=typescript)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-3-38B2AC?style=flat-square&logo=tailwind-css)

## Features

- **Sanity Studio** — headless CMS for managing articles, authors, and categories
- **Dynamic article pages** — server-rendered blog posts with rich content
- **Author profiles** — each post has a linked author with bio and image
- **Responsive layout** — clean reading experience on all screen sizes
- **Optimised images** — `@sanity/image-url` for responsive, CDN-delivered images
- **TypeScript throughout** — fully typed components and Sanity schemas

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | Next.js 14 (App Router) |
| CMS | Sanity v3 |
| Language | TypeScript 5 |
| Styling | Tailwind CSS, Styled Components |
| Image handling | @sanity/image-url |
| Deployment | Vercel (recommended) |

## Getting Started

### Prerequisites

- Node.js 18+
- A [Sanity](https://www.sanity.io) account (free tier works)

### Installation

```bash
git clone https://github.com/karan-sohi/Medium-clone.git
cd Medium-clone
npm install
```

### Sanity Setup

1. Create a Sanity project at [sanity.io](https://sanity.io)
2. Create a `.env.local` file:

```env
NEXT_PUBLIC_SANITY_PROJECT_ID=your_project_id
NEXT_PUBLIC_SANITY_DATASET=production
NEXT_PUBLIC_SANITY_API_VERSION=2024-01-01
```

### Run

```bash
# Start the Next.js app
npm run dev

# Start Sanity Studio (in a separate terminal)
npx sanity dev
```

- App: [http://localhost:3000](http://localhost:3000)
- Studio: [http://localhost:3333](http://localhost:3333)

### Deploy

The easiest deployment is [Vercel](https://vercel.com). Add your Sanity environment variables in the Vercel dashboard.

## Project Structure

```
├── app/              # Next.js App Router pages
├── components/       # Reusable React components
├── sanity/           # Sanity schemas & config
└── src/              # Utilities and helpers
```

## License

MIT
