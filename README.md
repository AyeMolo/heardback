# Heardback
job Search helper

## Problem
You apply, get an automated confirmation email, and then nothing. Weeks later you still don't know if anyone read your application, whether to follow up or if the job was ever real. Most people track this in a messy spreadsheet, if at all, and have no data on which companies actually respond.

## What Headback does

- **Application Tracker:** Forward your job emails to Heardback and it automatically records the company, role and status of every application (applied, assessment, interview, rejected). Applications with 30 days of silence are marked "likely ghosted."

- **Follow-Up Autopilot:**

- **Referral Path Finder:** Upload your LinkedIn connections export and contacts, and Heardback shows who you know at each company and drafts a natural outreach message.
- **Ghost Job Detector:** A Chrome extension that labels job postings as likely real, uncertain, or likely ghost, with a short explanation.

## What's different 
Existing ghost-job tools guess based on the posting alone. Heardback uses real outcomes: anonymized data from tracked applications shows how often a company actually responds (for example, "this company replied to 3% of applicants within 60 days"). The same data measures whether follow-ups and referrals really improve response rates.

## Status
Early development. Currently setting up the project and building a labeled test set of real job emails for the classifier.

## Stack 
- **Python:** email classification and AI work
- **Next.js:** web app, Self-hosted
- **Postgres:** database
- **LLM API:** classifying emails and drafting messages
- **Chrome extension:** capturing applications and showing ghost-job badges

## Privacy 

- Heardback stores only what it needs to track applications (company, role, status, dates), not your whole inbox.
- Sensitive data is encrypted.
- No LinkedIn scraping; connections come only from files you upload yourself.
- One click deletes everything Heardback has about you.