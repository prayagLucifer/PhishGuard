PhishGurad — Defender Academy
A browser-based cybersecurity training academy that helps learners recognize phishing through practical labs, simulated investigations, CTF-style challenges, assessments, badges, and certificates.

PhishGurad is an educational phishing-awareness and email-security training platform. It guides learners through realistic, fictional workplace scenarios and asks them to examine evidence, make security decisions, and explain their findings. The project is designed as an accessible learning prototype with a dark cyber-themed interface and a progression-based reward system.
Project status: Educational front-end prototype. The current version uses browser storage and does not include production authentication, a server-side database, or server-side certificate verification.

Features
Eight guided security labs
1. The Phishing Inbox — identify suspicious messages and practice inbox triage.
2. Anatomy of an Email — understand email fields and inspect message evidence.
3. URL Hunter — examine URL structure and identify the domain controlling a link.
4. Attachment Undercover — assess suspicious file details and choose safe handling steps.
5. Header Forensics: The Spoofed Identity — investigate sender identity and SPF, DKIM, and DMARC results.
6. Social Engineering: The Human Trap — recognize manipulation and plan a safe response to business email compromise scenarios.
7. Threat Intelligence & IOC Investigation — classify and correlate domains, IP addresses, and file hashes.
8. Operation PhishStorm — bring the evidence together in a final simulated SOC incident-response scenario.
Each lab contains three practical decision tasks and five knowledge-check questions. A learner earns the lab's certificate after all required answers for that lab are correct.
Learning paths
Three connected learning paths organize the labs into beginner, intermediate, and advanced stages:
- Phishing Fundamentals (Labs 01–03)
- Email & Human Threat Investigation (Labs 04–06)
- SOC Threat Response (Labs 07–08)
Challenges
The Challenges area contains four optional CTF-style missions. These use fictional evidence and an allow-listed simulated command runner; commands are not executed by the user's operating system.
Badges and certificates
- X-Access badge: awarded when a learner creates a demo account.
- Eight lab badges: each badge is awarded the first time the learner starts its corresponding lab.
- Eight lab certificates: each unlocks after the learner correctly completes that lab's three practical tasks and five knowledge questions.
- Main academy certificate: unlocks after all eight labs are complete and the learner passes the final exam with at least 80/100.
The final exam contains 20 multiple-choice questions and eight practical stations. Each practical station includes a simulated command task and a written analyst finding. Written responses are evaluated using predefined criteria in the prototype, not by a human assessor or an AI model.
Technology
- HTML5
- CSS
- JavaScript (vanilla)
- Tailwind CSS via CDN
- Three.js for the landing-page visual
- Lucide icons
- Google Fonts
- Browser localStorage for demo account details, progress, badges, and award state
Run locally
This is a front-end project. No build step or package installation is required for the current demo.
1. Clone or download this repository.
2. Open the main HTML file in a modern browser, or open the repository in Visual Studio Code and run it with the Live Server extension.
3. Create a demo account to receive the X-Access badge.
4. Start a lab to receive its badge, then complete its tasks and questions to unlock the corresponding certificate.
5. Complete all eight labs, take the final exam, and score at least 80/100 to unlock the main academy certificate.
For GitHub Pages, place the website file at the repository root and name it index.html, then enable GitHub Pages for the repository's publishing branch/folder.
Demo data and reset
The prototype stores demo account and learning progress in the browser's localStorage. This means progress is local to the browser and device where it was created; it is not synchronized between users or devices. Clearing the browser's site data will remove the locally stored demo account and progress.

To test the experience with a fresh profile, use a separate browser profile or clear the site's local storage for the PhishGurad page.
Important security and deployment notes
This repository is a learning prototype, not a production authentication or certification service.
- The account flow is a local demo and must be replaced with a secure backend authentication system before public production use.
- Do not enter real passwords or sensitive personal information into the demo.
- Progress and award checks are performed in the browser and can be modified by a user with browser developer tools. Production awards should be validated server-side.
- Add server-side certificate IDs, verification pages, and tamper-resistant records before treating certificates as official credentials.
- The project loads some libraries, icons, and fonts from CDNs, so those resources require an internet connection.
- The phishing emails, indicators, domains, and incident evidence used in the training scenarios are fictional examples for education.
- The PhishGurad academy certificate is an internal project credential; it is not an externally accredited industry certification.
Contributing
Contributions are welcome. Before submitting a pull request, please describe the change, identify the affected lab or section, and test the relevant learner flow in a browser. Avoid changing unrelated sections or award rules without documenting the reason.
License
No license has been selected yet. Add a LICENSE file before allowing others to reuse, modify, or distribute this project under explicit terms.
