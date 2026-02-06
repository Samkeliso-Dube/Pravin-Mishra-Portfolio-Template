# DMI Portfolio Website (Static HTML/CSS)

This repository contains a clean, professional-looking **static portfolio website** used in **DevOps Micro Internship (DMI)** Week 1 to practice:
- Linux basics
- Nginx hosting
- Deployment proof / ownership
- Production-style checks

✅ Students deploy this website on an Ubuntu VM using Nginx and keep it live for 24 hours.

---

## Who is this for?
- DMI students (beginner → intermediate)
- Anyone learning how to host a static site with Nginx on Linux

---

## What you will build
A portfolio-style website hosted on:
- **Ubuntu VM**
- **Nginx**
- Accessible via: `http://<public-ip>`

---

## Mandatory Ownership Proof (DMI Rule)
Before you deploy, you MUST edit the footer and add your details:

Original:

```html
<p>Crafted with <span>cloud</span> excellence by Pravin Mishra</p>
```

Add this line (example):

```html
<p><strong>Deployed by:</strong> DMI Cohort 2 | Rahul Sharma | Group 4 | Week 1 | 16-01-2026</p>
```

✅ This proof must be visible in your browser screenshot submission.

## Footer Version & Deploy Date

The footer displays:
Pravin Mishra Portfolio v1.0 — Deployed on <current date> — By Samkeliso

The deploy date is generated dynamically using JavaScript, so it always shows the current date when the site loads.

This change was implemented as part of a 5-day Jira sprint and deployed to the EC2 instance.

Pravin Mishra Portfolio v1.0 — Deployed on ```<span id="deployDate"></span>``` — By Samkeliso

```
<script>
const d = new Date();
document.getElementById("deployDate").innerText =
d.toLocaleDateString('en-GB', { day:'2-digit', month:'short', year:'numeric' });
</script>
```
