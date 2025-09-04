📘 Mini Finance UI

✨ A simple job listing web app deployed on AWS EC2.
This project is part of my DevOps and Cloud Engineering journey, where I practice version control, CI/CD basics, and cloud deployments step by step. It is powered by the training and guidance of Pravin Mishra, a great AWS DevOps guru.

🚀 Project Overview

The goal was to deliver a visible Mini Finance footer that shows version, deploy date, and author. Each day of the sprint added a small but meaningful improvement, just like in real DevOps workflows.

🗂 Sprint Goal

Ship a visible Mini Finance footer (version + date + author) to EC2 and document progress daily.

✅ Acceptance Criteria

Footer displays: Mini Finance v1.0 - Deployed on <DD Mon YYYY> - By Nkechi Ahanonye

Visible on all pages (homepage, about, contact, job listings)

Verified on public EC2 URL

📅 Daily Progress
Day 1 - Static Footer

Added footer with version, deploy date, and author

Pushed to GitHub and deployed to EC2

Verified footer is visible on live site

Day 2 - Dynamic Date

Updated footer to show date programmatically

Pushed changes and redeployed

Documented progress with snippet and screenshot

Day 3 - Polish and Accessibility

Improved footer styling (spacing, font size, background)

Checked accessibility contrast meets standards

Tested both desktop and mobile views

Hardcoded deploy date as 04 Sep 2025 for clarity

Day 4 - Provenance and Health Check

Added a /healthz endpoint returning OK

Verified with both browser and curl

Ensured EC2 app continued working smoothly

Day 5 - Review and Retrospective

Recorded a short demo video of EC2 app

Captured Jira burndown chart showing sprint progress

Wrote reflections on what went well and what to improve

🔎 Evidence

Screenshots: Footer displayed consistently on EC2 site

Browser and Curl: /healthz working as expected

Jira Story Link: Acceptance criteria, subtasks, and daily comments tracked

Burndown Chart: Clear sprint tracking from start to finish

Demo Video: Walkthrough of project hosted on EC2

📖 Retrospective
What went well

Small daily increments kept progress visible

GitHub to EC2 workflow now feels natural

Learned how to balance UI polish with ops visibility

What could be improved

Better date handling (hardcoding was only a temporary fix)

Next time I will set up automated deployment instead of manual copy to /var/www/html

Values practiced

Focus: One clear goal daily

Commitment: Completed the sprint without skipping

Openness: Shared blockers and solutions openly

Courage: Faced and fixed errors (Git SSH, EC2 reset)

Respect: Honored my mentor’s input and valued the learning

🛠 How to Run This Project
Run Locally

Clone the repo:

git clone https://github.com/nkydigitech/mini-finance-ui.git
cd mini-finance-ui


Open index.html in a browser

Footer should display version, deploy date, and author

Run on EC2

Launch an Ubuntu EC2 instance

Install web server (Nginx example):

sudo apt update
sudo apt install nginx -y


Copy project files:

sudo cp -r ~/mini-finance-ui/* /var/www/html/
sudo systemctl restart nginx


Visit: http://<EC2-Public-IP>

Verify footer and /healthz endpoint

📜 Commit History (Changelog)

Day 1: Add static footer with version, date, and author

Day 2: Update footer to dynamic date

Day 3: Polish footer styling and accessibility, hardcode date 04 Sep 2025

Day 4: Add /healthz endpoint for health check

Day 5: Final touches, retrospective notes, and demo prep

🙏 Acknowledgment

This project was powered by the teachings of Pravin Mishra, a great AWS DevOps guru, whose mentorship shaped my understanding and confidence in DevOps practices.

🔥 Built with love, persistence, and curiosity by Nkechi Ahanonye.
=======
# Mini Finance UI

A simple job listing web app deployed on AWS EC2.  
This project is part of my DevOps & Cloud Engineering journey, where I practice version control, CI/CD basics, and cloud deployments step by step.  

This DevOps class is powered by **Pravin Mishra**, a great AWS DevOps Guru, whose mentorship has guided me in building confidence and skill in real-world DevOps practices.  

---

## 🚀 Project Setup
- Frontend files (HTML, CSS, JS) hosted on **AWS EC2 (Ubuntu 24.04)**
- Web server: **Nginx**
- Source code managed with **Git + GitHub**
- Deployments done manually via **Git push + copy to EC2**
- Health check page: `/healthz.html`

---

## 📅 Daily Progress

### ✅ Day 1
- Cloned starter template into EC2  
- Initialized Git repository and pushed to GitHub  
- Deployed first version of the website on EC2  

### ✅ Day 2
- Created `healthz.html` file for status checks  
- Verified accessibility via `curl http://<EC2-IP>/healthz.html`  
- Updated README with progress notes  

### ✅ Day 3
- Hardcoded footer across HTML pages with deployment date:  
  *Mini Finance v1.0 | Deployed on 04 Sep 2025 | By Nkechi Ahanonye*  
- Staged, committed, and pushed changes to GitHub  
- Synced files to EC2 and confirmed deployment  

### ✅ Day 4
- Added commit hash and `/healthz.html` for verification  
- Browser and `curl` evidence captured to show app was responding correctly  
- Jira story updated with acceptance criteria, subtasks, and comments  

### ✅ Day 5
- Prepared README with full project history  
- Captured demo video of app running live on EC2  
- Project fully documented and submitted  

---

## 🔎 Verification Evidence

- **Browser check:** EC2 public IP displays Mini Finance UI  
- **Health check:**  
  ```bash
  curl http://<EC2-IP>/healthz.html

