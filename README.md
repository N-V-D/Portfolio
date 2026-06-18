# Portfolio
Personal Portfolio

# 🐛 Niranjan Desai | QA Engineer Portfolio

A dark, cinematic, terminal-inspired portfolio website built for a QA Engineer — designed around a "bug hunter" theme with live test-run animations, an interactive testing-process flow, and a contact form styled as a bug-report ticket.

**Live demo:** _add your deployed link here (e.g. Vercel / Netlify / GitHub Pages)_

---

## ✨ Features

- **Terminal boot-up loading screen** with animated typed lines
- **Animated particle network background** rendered on canvas
- **Dark / light mode toggle** with preference saved in `localStorage`
- **Fully responsive design** across mobile, tablet, and desktop
- **Sticky glassmorphism navbar** with active-link highlighting and mobile slide-in menu
- **Live "bug detector" console** widget
- **Animated stat counters** and skill progress bars
- **Interactive testing-process flow** (click each phase to see details)
- **Flip-card project tickets** styled like issue-tracker cards
- **Working contact form** powered by [EmailJS](https://www.emailjs.com/) — messages are sent directly to email, no backend required
- **Easter egg** hidden in the footer 🎉

---

## 🧰 Tech stack

| Category | Tools |
|---|---|
| Markup / Styling | HTML5, CSS3 (custom properties, animations, responsive grid/flexbox) |
| Scripting | Vanilla JavaScript |
| Fonts | [Inter](https://fonts.google.com/specimen/Inter), [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) via Google Fonts |
| Contact form | [EmailJS](https://www.emailjs.com/) (`@emailjs/browser`) |

No frameworks, build tools, or dependencies — it's a single static `index.html` file.

---

## 📁 Project structure

```
.
├── index.html                  # Main portfolio page (HTML + CSS + JS)
└── Niranjan_Desai_Resume.pdf   # Downloadable resume (linked from the hero section)
```

---

## 🚀 Getting started

### Run locally

1. Clone the repository
   ```bash
   git clone https://github.com/N-V-D/Portfolio.git
   cd Portfolio
   ```
2. Open `index.html` directly in your browser, or serve it locally:
   ```bash
   npx serve .
   ```

No build step or dependencies required.

### Deploy

This is a static site, so it can be deployed directly to any static hosting platform:
- **GitHub Pages** — enable Pages in repository settings, pointing to the root or `main` branch
- **Vercel** / **Netlify** — import the repo and deploy with default static settings

---

## 📧 Contact form setup (EmailJS)

The contact form sends submissions straight to email using EmailJS, so no backend server is needed.

1. Create a free account at [emailjs.com](https://www.emailjs.com/)
2. Add an email service (e.g. Gmail) and note the **Service ID**
3. Create an email template and note the **Template ID**
4. Copy your **Public Key** from the EmailJS dashboard
5. In `index.html`, update the following with your own credentials:
   ```js
   emailjs.init('YOUR_PUBLIC_KEY');

   const response = await emailjs.send(
     'YOUR_SERVICE_ID',
     'YOUR_TEMPLATE_ID',
     formData
   );
   ```

> **Note:** the template ID in this repo is currently a placeholder — replace `'YOUR_TEMPLATE_ID'` with your actual EmailJS template ID before deploying, or form submissions will fail.

---

## 🧩 Sections

- **Home** — intro, live status pill, quick QA stats
- **About** — bio, animated stat counters, QA mindset and focus areas
- **Skills** ("Weapons Arsenal") — automation stack, manual/regression testing, performance testing, daily QA toolkit, and an interactive testing-process flow
- **Projects** ("Case Files") — flip cards for SauceDemo, AnalytIQ Learning, Book Store Management System, and Art Gallery website, each with tech stack and bug summary
- **Experience** ("Test Run Log") — education and internship timeline
- **Certifications** ("Achievements Unlocked") — manual & automation testing, UI/UX, and technical writing certificates
- **Contact** ("File a Bug Report") — EmailJS-powered contact form plus direct email, phone, LinkedIn, GitHub, and WhatsApp links

---

## 📬 Connect with me

- **Email:** desainiranjan120@gmail.com
- **LinkedIn:** [niranjan-desai-992281326](https://www.linkedin.com/in/niranjan-desai-992281326/)
- **GitHub:** [N-V-D](https://github.com/N-V-D)
- **Location:** Pune, Maharashtra, India

---

## 📄 License

This project is open for reference and learning purposes. If you'd like to reuse parts of the design, please credit the original author.

---

<p align="center">Built with precision. Tested with obsession. 🐛</p>
