<div align="center">
  <img src="https://konomi.cz/konomiLogoRoundedSmall.png" width="72" alt="Konomi" />
  <h1>Richard Polanka</h1>
  <p>
    I build <b><a href="https://konomi.cz">Konomi</a></b>, a learning platform for economics, finance and IT<br/>
    used by Czech schools, teachers and students.<br/>
    Economics student at <b>VŠE Prague</b>.
  </p>
</div>

---

## Konomi

> Money isn't taboo. Economics isn't boring.

Financial literacy in Czech schools is usually taught from photocopies and slide decks, and
almost nobody finishes those. Konomi turns the same material into something students actually
get through: short lessons laid out on a path, hearts and streaks that keep momentum, and
interactive widgets where you move a slider and watch inflation quietly eat your savings.

|  | |
|---|---|
| **Students** | Courses on taxes, personal budgeting, investing, trading, pensions, marketing, law, central banking and digital circuits. Free to start, no card. |
| **Teachers** | Classes, assignments that mark themselves complete from real lesson progress, class leaderboards, a teacher's guide. |
| **Schools** | Their own course studio, white-label content, managed student accounts, per-seat licensing. |

**[konomi.cz](https://konomi.cz)** · [Courses](https://konomi.cz/prehled-kurzu) · [For schools](https://konomi.cz/skoly) · [Pricing](https://konomi.cz/cenik) · [Blog](https://konomi.cz/blog)

### How it is built

`Next.js 16 App Router` `TypeScript` `Drizzle ORM` `Neon Postgres` `Better Auth` `next-intl` `Tailwind` `shadcn/ui` `Stripe` `Vercel`

Roughly 144k lines of TypeScript across ~790 files, designed, written and shipped solo.
The parts I am most happy with:

- **Content engine.** A lesson is a TipTap document, and interactive widgets (compound interest,
  tax and budget calculators, market simulators) are first-class nodes inside it, so new course
  material is authored rather than hard-coded.
- **Challenger.** A game layer on top of the courses: word of the day, leaderboards, and a
  map-based territory battle where students fight over regions of the country.
- **Multi-tenant schools.** Organizations with their own courses, admins, student accounts and
  billing, living in the same database as the public platform without leaking into it.
- **One progress model.** Hearts, gems, stars, streaks and assignment completion are all derived
  from the same activity events, so a lesson finished anywhere counts everywhere.

---

## Elsewhere

Most of what I write lives in private repositories. What is public here is older and smaller:

- **[digit_recognition_app](https://github.com/richardpolanka/digit_recognition_app)** — handwritten digit recognition, PyTorch + FastAPI
- **[mcs51docs](https://github.com/richardpolanka/mcs51docs)** — documentation for the MCS-51 microcontroller
- **[task-manager-gitops](https://github.com/richardpolanka/task-manager-gitops)** — GitOps configuration for a Kubernetes task manager
- **[portfolio](https://github.com/richardpolanka/portfolio)** — an earlier personal site

Before Konomi I spent my time on finance, security and a handful of client projects, which is
roughly how I ended up wanting to teach the first two.

---

<div align="center">
  <a href="mailto:richard.polanka@gmail.com"><img src="https://img.shields.io/badge/email-2BAB90?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://www.linkedin.com/in/richard-polanka-275041197/"><img src="https://img.shields.io/badge/linkedin-2BAB90?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://x.com/richard_polanka"><img src="https://img.shields.io/badge/x-2BAB90?style=flat-square&logo=x&logoColor=white" alt="X" /></a>
  <a href="https://konomi.cz"><img src="https://img.shields.io/badge/konomi.cz-2BAB90?style=flat-square&logo=vercel&logoColor=white" alt="konomi.cz" /></a>
</div>
