# HLSA SecOps AI Agency Website

## Project Overview

Multi-page marketing website for HLSA SecOps AI, the AI automation division of HLSA SecOps. Security-first AI automation agency. Static HTML files with embedded CSS and JavaScript—no build step required.

## Related Sites

- **Parent Company**: https://hlsasecops.com
- **AI Division**: https://ai.hlsasecops.com (target deployment)

## Tech Stack

- **Framework**: Static HTML (no build step)
- **Styling**: Embedded CSS
- **JavaScript**: Vanilla JS, embedded
- **Hosting**: Netlify
- **Fonts**: Inter (Google Fonts CDN)

## File Structure

```
├── index.html          # Main landing page (hero, case studies, process, services overview)
├── services.html       # Detailed services page (Lead Gen, Operations, AI Agents, Sales Admin, Pricing)
├── about.html          # About page (story, founders, timeline, values)
├── contact.html        # Contact page (form with Netlify Forms, contact info)
├── netlify.toml        # Netlify configuration
├── CLAUDE.md           # This file
```

## Design System

### Colors
| Token | Hex | Usage |
|-------|-----|-------|
| Black base | `#0A0A0B` | Background |
| Dark surface | `#0f0f11`, `#161618` | Cards, sections |
| Teal primary | `#4499A0` | Primary accents, CTAs |
| Teal bright | `#5ab8c0` | Hover states |
| Teal dark | `#357a80` | Active states |
| Gold primary | `#D88E26` | Secondary accent, stats |
| Gold bright | `#e8a43e` | Hover states |

### Typography
- **Font**: Inter
- **Weights**: 300-800
- **Letter spacing**: -0.03em (tight)

### Corner Radii
Squared/luxe aesthetic — avoid rounded pills:
- Small: `4px`
- Medium: `6px`
- Large: `8px`

### Logo
Text wordmark: "HLSA" in white, "SecOps" in teal (`#4499A0`), "AI" in gold (`#D88E26`).

## Brand Voice

- **Tagline**: "Stay Offensive."
- **Tone**: Direct, confident, security-aware
- **Key phrases**: "Security-first", "locked down", "stay offensive", "bulletproof"
- **Positioning**: AI automation agency with cybersecurity roots

## Page Structure

### index.html (Main Landing Page)
1. **Hero** — "AI automation that stays offensive" with teal/gold gradient orbs
2. **Social Proof** — Scrolling platform ticker (Make, n8n, OpenAI, etc.)
3. **Case Studies** — 3 cards (Financial Services, Healthcare, SaaS)
4. **How It Works** — 3-step process (Security Briefing, Architecture, Build & Deploy)
5. **Services Overview** — 6 cards (Workflow, AI Agents, Data Pipelines, Chatbots, Reporting, Security)
6. **CTA** — "Ready to automate without compromise?"
7. **Footer** — Logo, nav links, copyright

### services.html (Detailed Services)
1. **Hero** — Stats-focused (150+ systems, 98% retention, 0 breaches)
2. **Lead Generation Systems** — AI Cold Outreach, Application Funnels, Content Systems
3. **Operations Automation** — Automated Fulfillment, Client Onboarding, PM Workflows
4. **AI Agent Systems** — Customer Support, Data Analysis, Compliance Agents
5. **Sales Administration** — Smart CRM, AI Proposals, Nurture Sequences
6. **Who It's For** — Healthcare, Financial Services, SaaS, Professional Services
7. **Process** — 4-step timeline (Discovery, Design, Build, Launch)
8. **Pricing** — Three tiers (Single System $5K, Growth Package $12K, Retainer $5K/mo)
9. **CTA** — Final call-to-action

### about.html (About)
1. **Hero** — "Built by operators who stay offensive"
2. **Story** — From cybersecurity to AI automation narrative
3. **Leadership** — Founder and security team cards
4. **Timeline** — 2021-2025 milestones
5. **Values** — 6 principles (Security First, Results Over Hype, etc.)
6. **CTA** — Call-to-action

### contact.html (Contact)
1. **Hero** — "Let's talk security-first automation"
2. **Contact Form** — Name, email, company, industry selector, message (Netlify Forms)
3. **Contact Info** — Email, call scheduling, security/privacy note, location
4. **Footer**

## Interactive Features

- Scroll-triggered reveal animations via Intersection Observer
- Animated counters with easeOutQuart easing
- Mouse-following cursor glow effect (desktop only)
- Scroll progress indicator in header (teal-to-gold gradient)
- Smooth scroll navigation
- Mobile hamburger menu (index.html)
- Netlify form handling with success state (contact.html)
- Fully responsive down to mobile

## Deployment

### Deploy to Production
```bash
netlify deploy --prod
```

### Preview Deploy
```bash
netlify deploy
```

## Contact Information

- **Email**: info@hlsasecops.com
- **Parent Site**: https://hlsasecops.com

## Common Tasks

### Update Colors
- Teal primary: `#4499A0`
- Teal bright: `#5ab8c0`
- Gold primary: `#D88E26`
- Gold bright: `#e8a43e`

### Update Pricing (services.html)
Find the `.pricing-card` elements. Each has `.pricing-name`, `.pricing-amount`, and `.pricing-features`.

### Update Contact Email
Search for `info@hlsasecops.com` across all files.

## Notes

- Keep the single-file architecture — no bundlers or build steps
- Maintain the squared corner aesthetic (no pills)
- Security-first messaging throughout all copy
- Test scroll animations after content changes
- **index.html is the main landing page** — don't overwrite with feature content
