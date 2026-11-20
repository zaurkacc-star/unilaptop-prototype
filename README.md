# UniLaptop: Laptop Lending and Support Platform (Prototype)

Final Project, Business Analysis course, Astana IT University
Team 5, group ITM-2402: Viktor Shalamov, Almaz Alikeev, Zaur Kasmukhanov, Baktiyar Murzagaliev
Instructor: Nurkhat Ibadildin

**Demo video:** [Team05_FP_Demo.mp4][video]
**Live demo:** [jazzy-kulfi-8222f1.netlify.app](https://jazzy-kulfi-8222f1.netlify.app/)

## What it is

An interactive prototype of the UniLaptop platform described in our SRS. A company owns laptops,
the university pays a subscription, and students borrow laptops for free. The prototype shows the
main use case: a student requests a laptop, the issuance office approves it and issues it with a
digital transfer act, and the IT administrator handles incidents with consent-based remote support.

## Files

| File | Content |
|---|---|
| `index.html` | The whole prototype: HTML, CSS and JavaScript in one file |
| `README.md` | This file |

## Technology

- Plain HTML, CSS and JavaScript in one page, no build step.
- Interface in Russian, Kazakh and English.
- Data is stored in the browser (`localStorage`), so requests are kept between roles and between
  browser tabs.
- University Student Records, notifications.
- Icons are loaded from the Font Awesome CDN.

## How to run

The prototype is meant to be run on **Netlify**.

The quickest way is to open the live demo link above. To deploy your own copy:

1. Go to https://app.netlify.com/drop and sign in.
2. Drag the folder with `index.html` into the page.
3. Netlify publishes the site in a few seconds and gives a link like `https://<name>.netlify.app`.
4. Open the link in Chrome, Edge or Firefox.

The file must be named `index.html`, otherwise Netlify does not open it as the start page.

## Roles

On the login screen choose a role and press **Sign in**. All accounts and data are invented.

| Role | What it can do |
|---|---|
| Student | Request a laptop by study program, see request status and notices, report a problem |
| Issuance office staff | See incoming requests, approve or reject them, fill in and sign the transfer act |
| IT administrator | Monitor devices, handle support requests, start a remote session with consent |
| UniLaptop owner | See the whole fleet, utilization and demo financial figures |

## Main use case (as in the demo video)

1. Student signs in and requests a laptop configuration for the study program (FR-01, FR-02, FR-05).
2. Issuance office staff sign in, see the request in the incoming queue and approve it (FR-08, FR-09).
3. The student sees the approval notice and the request status (FR-10).
4. Issuance office staff fill in the digital transfer act with a condition checklist and signature (FR-12).
5. The student reports a problem; the request goes to the IT administrator (FR-17, FR-18).
6. The administrator starts a remote session only with the student's consent; personal files stay hidden and the session is logged (FR-22, FR-25).

To see that the data is saved, open the prototype in two tabs of the same browser: sign in as a
student in one tab and as issuance office staff in the other. A new request appears in the staff
queue without reloading the page.

## Data and privacy

All names, IDs and devices are invented test data. No real passwords or personal data are used.

[video]: https://astanait-my.sharepoint.com/:v:/r/personal/243136_astanait_edu_kz/_layouts/15/stream.aspx?id=%2Fpersonal%2F243136_astanait_edu_kz%2FDocuments%2FTeam05_FP_Demo.mp4&share=cQrYQ8TeRn2YT6i3fOd-nQCrEgUC3StktRghTw8MIffR5NsRfw&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0
