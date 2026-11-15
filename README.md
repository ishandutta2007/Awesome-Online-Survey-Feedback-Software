# Awesome-Online-Survey-Feedback-Software

# Awesome Online Survey & Feedback Software

> A curated list of top Online Survey and Feedback Software platforms — both SaaS/Hosted commercial solutions and open-source alternatives for creating forms, collecting responses, and analyzing feedback.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
- [Open-Source Software](#-open-source-software)
- [Comparison at a Glance](#-comparison-at-a-glance)
- [Contributing](#-contributing)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Online Survey and Feedback Software platforms. These are not open-source but are included as reference points for feature comparison.

| Platform | Company Size (Valuation / Revenue) | Starting Price | Free Tier Limit | Description |
| :--- | :--- | :--- | :--- | :--- |
| **Google Forms** | ~$2.1T+ market cap / ~$350B+ ann. rev (Alphabet) | $7/user/month (via Google Workspace Business Starter; standalone tool is $0) | Free forever (Unlimited surveys and responses; limited only by 10M cell Google Sheet limit and 15 GB shared Google Drive storage) | Free, simple form builder within Google Workspace integrated with Google Sheets for response collection. |
| **Qualtrics CoreXM** | $13B acquisition valuation / ~$1.4B+ ann. rev | $420/month ($5,040/year billed annually for self-serve Strategic Research; CoreXM enterprise starts ~$25,000–$50,000/year) | Free forever (500 total lifetime responses, up to 3 active surveys, max 30 questions per survey, 1 user) | Enterprise experience management platform providing sophisticated statistical analysis and multi-channel feedback collection. |
| **SurveyMonkey** | ~$4.1B peak valuation (STG acquisition) / ~$480M+ ann. rev | $39/month (billed annually at $468/yr) or $149/month (billed monthly) | Free forever (10 questions per survey, 40 viewable responses per survey, unlimited surveys, no data export) | Industry-standard survey platform offering extensive template libraries, logic branching, and analytics. |
| **Typeform** | $935M valuation (Series C) / ~$90M+ ARR | $28/month (billed annually) or $39/month (billed monthly) | Free forever (10 responses/month across all forms, unlimited forms) | Conversational, design-focused form builder popularized for one-question-at-a-time form experience. |
| **Alchemer** | ~$400M–$500M valuation (KKR-backed) / ~$40M+ ARR | $55/user/month (billed monthly) or $26.25/user/month ($315/year billed annually) | 7-day free trial (Full evaluation access to features and response collection; no credit card required) | Enterprise survey platform with advanced logic, custom workflows, and deep reporting. |
| **Jotform** | Bootstrapped ($0 VC raised) / ~$145M+ ann. rev | $34/month (billed annually) or $39/month (billed monthly) | Free forever (5 active forms, 100 submissions/month, 500 total stored submissions, 100 MB storage, 10 payment submissions/month) | Form builder with extensive integrations, drag-and-drop builder, and payment support. |

---

## 🟩 Open-Source Software

Self-hosted, community-driven Online Survey and Feedback Software tools. The open-source ecosystem spans **mature GPL survey platforms**, **modern AGPL experience management suites**, and **Typeform-style form builders**.

### LimeSurvey
**Stack:** PHP / MySQL/PostgreSQL/MariaDB/MSSQL | **License:** GPL v2.0[citation:5][citation:6]
LimeSurvey is the most established open-source survey platform, in development since 2006 and used in 80+ countries[citation:5][citation:6]. It is explicitly positioned as a free alternative to SurveyMonkey, Typeform, Qualtrics, and Google Forms[citation:1]. Key features include:
- **Unlimited surveys and questions** with 30+ question types and 900+ templates[citation:5]
- **Advanced logic**: skip logic, question branching, and conditional questions[citation:5]
- **Multilingual support** for 80+ languages[citation:5]
- **On-brand surveys** with customizable fonts, colors, logos, CSS, and JavaScript[citation:5]
- **GDPR compliance**, data anonymization, and WCAG 2.0 accessibility[citation:5]
- **Extensibility** via plugins, RemoteControl API (XML-RPC/JSON-RPC), and integrations with SAML, LDAP, and REST API[citation:5]

Deployment requires a LAMP-style stack with PHP 8.2+ and a supported database[citation:6]. A hosted SaaS option is available for teams not wanting to self-host[citation:5].
**Best for:** Organizations wanting a proven, feature-rich open-source survey platform with advanced logic, multilingual support, and GDPR compliance, accepting the PHP/database deployment overhead.

### Formbricks
**Stack:** TypeScript / Next.js / PostgreSQL / Redis | **License:** AGPLv3 (core) / Enterprise (separate)[citation:14]
Formbricks is the leading open-source **experience management (XM) suite**, explicitly positioned as an open-source alternative to Qualtrics, Typeform, SurveyMonkey, and Google Forms[citation:3][citation:10]. It goes beyond simple surveys with:
- **In-app surveys** with precise user targeting based on attributes, events, and segments[citation:10]
- **Website surveys** embeddable via JavaScript snippet[citation:10]
- **Link surveys** with custom branding and shareable URLs[citation:10]
- **20+ question types** including NPS, CES, CSAT, matrix, ranking, and file upload[citation:10]
- **Skip logic and conditional branching**[citation:10]
- **Built-in analytics** with charts and CSV/JSON export[citation:10]
- **Integrations** with Slack, Notion, Google Sheets, Airtable, Zapier, and n8n[citation:10]

Self-hosting is available via Docker with PostgreSQL (pgvector-enabled) and Redis[citation:10]. The core is AGPLv3, with enterprise features requiring a license key[citation:14]. A hosted cloud version with a generous free plan is also available.
**Best for:** Product teams wanting in-app and website surveys with precise targeting and a modern UI, accepting the AGPL licensing and Docker deployment.

### OpnForm
**Stack:** Laravel / Nuxt / PostgreSQL / Redis | **License:** AGPL-3.0[citation:9]
OpnForm is an open-source **Typeform alternative** with a drag-and-drop form editor, shareable links and embeds, conditional logic, and file uploads[citation:9]. It is positioned for contact forms, surveys, lead capture, and internal request forms. Self-hosting via Railway or Docker spins up the Laravel API, Nuxt frontend, PostgreSQL, and Redis[citation:9]. The free community edition allows 2 users, with additional users requiring a paid plan. Optional features include AI form generation via OpenAI API key and SMTP for email notifications[citation:9].
**Best for:** Teams wanting a Typeform-style form builder with conditional logic and file uploads, accepting the Laravel/Nuxt stack and AGPL licensing.

### QuillForms
**Stack:** React / TypeScript | **License:** Open Source (per GitHub topic)[citation:2]
QuillForms is an open-source **Typeform clone** built with React and TypeScript, focused on conversational multi-step forms[citation:2]. It is a WordPress plugin, making it the natural choice for WordPress sites needing Typeform-style forms. It has 581 GitHub stars and is actively maintained[citation:2]. As a WordPress plugin, it integrates natively with the WordPress ecosystem.
**Best for:** WordPress site owners wanting Typeform-style conversational forms without a separate platform, accepting the WordPress plugin dependency.

### OpenFlow
**Stack:** (Check repository) | **License:** Open Source[citation:13]
OpenFlow is a free, open-source alternative to landing-page lead generation form makers like Typeform, positioned for startups and SMEs[citation:13]. Key features include a drag-and-drop builder, iframe embed with auto-resize, editable URL slugs, custom subdomains, GTM integration with cookie consent, a WordPress plugin (shortcode, WPBakery, Gutenberg), Docker deployment with SQLite (no external DB), multi-user roles, white-label branding, API tokens, backup/restore with scheduled backups, audit logs, and two-factor login[citation:13]. It is designed for lead generation forms rather than complex surveys.
**Best for:** Startups and SMEs wanting a lightweight, self-hosted lead-gen form builder with strong embedding and branding options, accepting a narrower survey feature set.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Question Types | In-App/Website Surveys | Logic Branching | Self-Hosted | Best For |
|----------|---------|-------|----------------|------------------------|-----------------|-------------|----------|
| **SurveyMonkey** | Proprietary | Cloud | ✅ | ❌ | ✅ | ❌ | Industry-standard surveys |
| **Typeform** | Proprietary | Cloud | ✅ | ❌ | ✅ | ❌ | Conversational forms |
| **Qualtrics** | Proprietary | Cloud | ✅ | ❌ | ✅ Advanced | ❌ | Enterprise experience mgmt |
| **LimeSurvey** | GPL v2.0 | PHP/DB | ✅ 30+ | ❌ | ✅ | ✅ | Full-featured OSS surveys |
| **Formbricks** | AGPLv3 | Next.js/Postgres | ✅ 20+ | ✅ In-app + website | ✅ | ✅ | Open-source Qualtrics alt |
| **OpnForm** | AGPL-3.0 | Laravel/Nuxt | (Check) | ❌ | ✅ | ✅ | Typeform-style forms |
| **QuillForms** | Open Source | React/TS | (Check) | ❌ | ✅ | ✅ (WordPress) | WordPress conversational forms |
| **OpenFlow** | Open Source | (Check) | (Check) | ❌ | (Check) | ✅ | Lead-gen forms |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Online Survey or Feedback Software tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source.

**Note on the open-source ecosystem:** The survey and feedback space splits between **mature full-featured platforms** (LimeSurvey, with 20 years of development, 30+ question types, and 80+ languages[citation:5]) and **modern experience management suites** (Formbricks, explicitly targeting the Qualtrics/Typeform use case with in-app and website targeting[citation:10]). **LimeSurvey** is the strongest choice for complex, logic-heavy surveys and academic research, while **Formbricks** is the best fit for product teams wanting in-app NPS/CSAT surveys with user targeting. **OpnForm** and **QuillForms** fill the Typeform-style conversational form niche, with QuillForms being the WordPress-native option. No open-source project fully replicates the enterprise analytics depth of Qualtrics, but LimeSurvey and Formbricks cover the majority of practical survey and feedback needs.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
