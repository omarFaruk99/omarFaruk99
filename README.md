# Omar Faruk

**Software engineer. I build web applications and run them myself.**

I write the application and then own the part most developers hand off — the server,
the containers, the reverse proxy, the certificates, the deploy. Computer Science
background, currently at Innovate Solution.

---

## What I run

**[MailHub](https://github.com/omarFaruk99/mailhub)** — a self-hosted email marketing
platform, live at [mailhub.omarsec.com](https://mailhub.omarsec.com)

Built it, deployed it, and I keep it running. It replaced sending campaigns by hand from
WordPress, and now delivers 8,000–10,000 emails a month across multiple brands.

- Three Docker Compose services — Next.js, Express, PostgreSQL — all bound to `127.0.0.1`,
  reachable only through nginx with Let's Encrypt TLS
- Amazon SES for delivery; bounces and complaints return over SNS to a signature-verified
  webhook and suppress the address automatically
- Auto-pause acts as an emergency brake when bounce or complaint rates climb, and only a
  human can lift it
- Exactly-once sending enforced in the schema, so a retry or a crash can never email
  someone twice
- Migrations run on container start; `git pull && docker compose up -d --build` is the
  whole deploy

`TypeScript` · `Docker` · `PostgreSQL` · `Prisma` · `nginx` · `AWS SES` · `pg-boss`

**[omarsec](https://github.com/omarFaruk99/omarsec)** — infrastructure and security notes,
published at [omarsec.com](https://omarsec.com)

103 pages written while learning the ground under the applications I ship.

| Section | Pages |
| --- | --- |
| Linux fundamentals | 36 |
| Docker | 18 |
| Server deployment | 9 |
| AWS SES | 7 |
| Git and GitHub | 6 |
| CI/CD | 4 |
| Claude Code | 22 |

`Next.js` · `Nextra` · `MDX`

---

## What I work with

| | |
| --- | --- |
| **Infrastructure** | Docker, Docker Compose, nginx, Linux (Ubuntu), AWS EC2, AWS SES, Let's Encrypt, Cloudflare |
| **Backend** | Node.js, Express, TypeScript, PostgreSQL, Prisma, MongoDB, REST APIs |
| **Frontend** | React, Next.js, Astro, Tailwind CSS, TypeScript |
| **Practice** | Git, GitHub Actions, technical SEO, Core Web Vitals |

---

## Where I came from

Building web applications with React and Node, then technical SEO for a B2B travel API
company — schema, crawlability, Core Web Vitals, and a WordPress-to-static migration.

That turn is what pulled me toward infrastructure. Chasing page-load numbers means caring
about how something is served, not only how it is written. Owning a deploy is the same
question one layer down.

---

## Currently

- Migrating a WordPress blog to a static Astro build on Cloudflare Pages
- Adding a Dockerfile and a GitHub Actions pipeline to MailHub
- Writing up the Linux and Docker ground on omarsec.com as I go

---

## Contact

[LinkedIn](https://www.linkedin.com/in/omarfaruk99/) · [omarsec.com](https://omarsec.com) ·
2035faruk@gmail.com
