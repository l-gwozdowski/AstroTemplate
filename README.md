# Starter Template (Astro)

Reusable Astro baseline with a one-page homepage architecture and an additional blog module.

## What is included

- One-page homepage composed from reusable section components
- Sticky header with anchor navigation (`/#home`, `/#about`, `/#services`, `/#contact`)
- Additional blog powered by Astro Content Collections
- Accessible defaults (skip link, keyboard-safe mobile nav, semantic sections, visible focus states)
- Separate controls with persistence: `Light/Dark`, always-available `High Contrast` (black/yellow), and font size (`A-`, `A+`, `100%/130%`)
- `astro-icon` integration with Tabler icon set for UI icons
- Tailwind CSS v4 integration
- MDX and sitemap integrations

## Project structure

```text
src/
  components/
    BaseHead.astro
    FormattedDate.astro
    layout/
      Footer.astro
      Header.astro
      HeaderLink.astro
      Navigation.astro
      ThemeToggle.astro
    sections/
      home/
        HeroSection.astro
        AboutSection.astro
        FeatureSection.astro
        LatestPostsSection.astro
        CtaSection.astro
  config/
    site.ts
  content/
    blog/
      *.md
      *.mdx
  layouts/
    BaseLayout.astro
    BlogPost.astro
  pages/
    index.astro
    blog/
      index.astro
      [...slug].astro
  styles/
    global.css
  content.config.ts
```

## Commands

```bash
npm install
npm run dev
npm run build
npm run preview
npm run astro -- check
```

## Customize quickly

1. Update metadata, navigation, and contact values in `src/config/site.ts`.
2. Replace homepage sections in `src/components/sections/home`.
3. Add posts in `src/content/blog`.
4. Tune colors and spacing in `src/styles/global.css`.
5. Review `ACCESSIBILITY.md` after each major UI/content change.

## Notes

- `astro.config.mjs` uses `https://example.com` as placeholder site URL.
- Replace that URL before production deploy.
- Remove blog routes and `src/content` if you need a pure one-page site.
