<h1 align="center">Omar Faruk</h1>

<p align="center">
  <b>Software engineer. I build web applications and run them myself.</b>
</p>

<p align="center">
  <a href="https://omarsec.com"><img alt="Website" src="https://img.shields.io/badge/omarsec.com-111827?style=for-the-badge&logo=googlechrome&logoColor=white"></a>
  <a href="https://www.linkedin.com/in/omarfaruk99/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"></a>
  <a href="mailto:2035faruk@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"></a>
</p>

<p align="center">
  I write the application and then own the part most developers hand off —<br>
  the server, the containers, the reverse proxy, the certificates, the deploy.<br>
  Computer Science background, currently at Innovate Solution in Dhaka.
</p>

---

## What I run

<table>
<tr>
<td width="50%" valign="top">

### [MailHub](https://github.com/omarFaruk99/mailhub)

A self-hosted email marketing platform. Built it, deployed it, and I keep it running.
It replaced sending campaigns by hand from WordPress, and now delivers **8,000–10,000
emails a month** across multiple brands.

![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![nginx](https://img.shields.io/badge/-nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![AWS SES](https://img.shields.io/badge/-AWS%20SES-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)

**[mailhub.omarsec.com →](https://mailhub.omarsec.com)**

</td>
<td width="50%" valign="top">

### [omarsec](https://github.com/omarFaruk99/omarsec)

Infrastructure and security notes — **103 pages** written while learning the ground
under the applications I ship. Linux, Docker, server deployment, AWS SES, CI/CD and
Git, published as a static site.

![Next.js](https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Nextra](https://img.shields.io/badge/-Nextra-111827?style=flat-square&logo=markdown&logoColor=white)
![MDX](https://img.shields.io/badge/-MDX-1B1F24?style=flat-square&logo=mdx&logoColor=white)
![Linux](https://img.shields.io/badge/-Linux-1A1A1A?style=flat-square&logo=linux&logoColor=white)
![Cloudflare](https://img.shields.io/badge/-Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white)

**[omarsec.com →](https://omarsec.com)**

</td>
</tr>
</table>

**Inside MailHub**

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

---

## Toolbox

<table>
<tr><td><b>Infrastructure</b></td><td>

![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![nginx](https://img.shields.io/badge/-nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![Linux](https://img.shields.io/badge/-Linux-1A1A1A?style=flat-square&logo=linux&logoColor=white)
![AWS](https://img.shields.io/badge/-AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Cloudflare](https://img.shields.io/badge/-Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/-GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

</td></tr>
<tr><td><b>Backend</b></td><td>

![Node.js](https://img.shields.io/badge/-Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/-Express-000000?style=flat-square&logo=express&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Prisma](https://img.shields.io/badge/-Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white)
![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)

</td></tr>
<tr><td><b>Frontend</b></td><td>

![React](https://img.shields.io/badge/-React-149ECA?style=flat-square&logo=react&logoColor=white)
![Next.js](https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Astro](https://img.shields.io/badge/-Astro-BC52EE?style=flat-square&logo=astro&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/-Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

</td></tr>
<tr><td><b>Practice</b></td><td>

Git · CI/CD · server hardening · technical SEO · Core Web Vitals

</td></tr>
</table>

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
