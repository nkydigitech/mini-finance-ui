# Mini Finance UI – Sprint 1 Footer Implementation

This README documents the full progress of adding the Mini Finance footer, from initial implementation to accessibility checks and deployment proof.

---

## Sprint Goal
Ship a visible Mini Finance footer (version + date + author) to EC2 and document progress daily.

---

## What We Did

### Day 1 – Initial Footer
**Date:** 02 Sep 2025  
We added a simple, static footer to all pages showing the version, deploy date, and author:
```html
<footer style="text-align:center; font-size:12px; padding:10px; background:#f1f1f1;">
  Mini Finance v1.0 — Deployed on 02 Sep 2025 — By Nkechi Ahanonye
</footer>

const today = new Date();
today.setDate(today.getDate() + 1);
const options = { day: '2-digit', month: 'short', year: 'numeric' };
document.getElementById('deploy-date').textContent = today.toLocaleDateString('en-GB', options);


const today = new Date();
today.setDate(today.getDate() + 1);
const options = { day: '2-digit', month: 'short', year: 'numeric' };
document.getElementById('deploy-date').textContent = today.toLocaleDateString('en-GB', options);


const today = new Date();
today.setDate(today.getDate() + 1);
const options = { day: '2-digit', month: 'short', year: 'numeric' };
document.getElementById('deploy-date').textContent = today.toLocaleDateString('en-GB', options);
