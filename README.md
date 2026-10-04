# code-catalystBuild a modern, responsive full-stack web application called “OpportunityHub” to solve the Hackathon Problem Statement 1: “The Opportunity Gap”.

PROBLEM:
Students receive information about internships, scholarships, hackathons, research opportunities, coding contests, workshops, fellowships and competitions through scattered WhatsApp groups, clubs, seniors, faculty, college cells and personal networks. Because the information is fragmented, students miss relevant opportunities, discover them too late, or cannot determine whether they are eligible.

GOAL:
Create a centralized, personalized and trustworthy opportunity discovery platform where students can discover relevant opportunities, verify information, save opportunities, track applications and receive deadline reminders.

IMPORTANT:
This is an MVP for a college hackathon. Prioritize a polished working demo and excellent user experience over unnecessary complexity.

==================================================
1. TECH STACK
==================================================

Use a modern web stack suitable for a hackathon.

Preferred:
- React
- TypeScript
- Tailwind CSS
- Modern component library such as shadcn/ui
- Supabase for authentication and database if backend functionality is required
- Use clean reusable components
- Make the application responsive for both mobile and desktop

If the environment already has a suitable stack configured, use the existing stack instead of unnecessarily changing it.

The application must actually work. Do not create fake buttons that do nothing.

==================================================
2. BRANDING
==================================================

Application name:
OpportunityHub

Tagline:
“Find the right opportunity before it’s too late.”

Create a professional student-focused visual identity.

Design should feel:
- Modern
- Clean
- Trustworthy
- Student-friendly
- Slightly futuristic
- Professional enough for a hackathon demo

Use cards, badges, subtle gradients, clean typography, icons and good spacing.

Do NOT make it look like a generic admin dashboard.

==================================================
3. LANDING PAGE
==================================================

Create an attractive landing page containing:

Hero section:
“Stop Missing Opportunities.”

Subtitle:
“Discover internships, scholarships, hackathons, research programs and competitions matched to you — all in one place.”

Primary CTA:
“Explore Opportunities”

Secondary CTA:
“Create My Profile”

Show visual statistics such as:
- 250+ Opportunities
- 50+ Verified Sources
- 10+ Opportunity Categories

Include a short explanation of the problem:
“Opportunities are everywhere. Information is not.”

Show how OpportunityHub solves it:

SCATTERED INFORMATION
→ ORGANIZED
→ VERIFIED
→ PERSONALIZED
→ DEADLINE TRACKED

Include feature cards:
1. Personalized Discovery
2. Verified Opportunities
3. Smart Matching
4. Deadline Alerts
5. Application Tracker
6. Community Contributions

==================================================
4. STUDENT ONBOARDING
==================================================

Create a simple profile setup flow.

Ask for:

- Name
- College
- Branch
- Year
- Skills
- Interests
- Preferred opportunity types
- Optional eligibility information

Example:
Name: Anshika
Branch: CSE
Year: 1st Year
Skills: C, Python, HTML/CSS
Interests: AI/ML, Web Development
Preferred opportunities:
- Hackathons
- Scholarships
- Internships
- Research

Allow users to edit their profile later.

==================================================
5. PERSONALIZED DASHBOARD
==================================================

After onboarding, show a student dashboard.

Top section:
“Good morning, [Name] 👋”

Then:

“Opportunities For You”

Each opportunity card should contain:

- Opportunity title
- Organization
- Category
- Short description
- Eligibility
- Deadline
- Days remaining
- Skills/tags
- Verification status
- Match percentage
- Save button
- Apply button

Example:

Google AI Hackathon

Google
🏆 Hackathon

92% Match

Why this matches you:
✓ CSE eligible
✓ 1st year eligible
✓ AI interest matches
✓ No previous experience required

Deadline:
12 Oct 2026

[Save] [Apply]

==================================================
6. OPPORTUNITY CATEGORIES
==================================================

Support:

- Internships
- Scholarships
- Hackathons
- Research
- Fellowships
- Coding Contests
- Competitions
- Workshops

Create category navigation/filtering.

==================================================
7. SEARCH AND SMART FILTERS
==================================================

Create a powerful search interface.

Search by:
- Opportunity name
- Organization
- Skill
- Category

Filters:
- Category
- Branch
- Year
- Skills
- Eligibility
- Paid/Unpaid
- Online/Offline
- Deadline
- Verified only

Sort by:
- Best Match
- Deadline Soon
- Recently Added
- Most Popular

The filtering must actually work.

==================================================
8. AI MATCHING
==================================================

Implement a simple intelligent matching system for the MVP.

Calculate a match percentage using the student's profile and opportunity information.

Example:

Student:
CSE
1st Year
Python
AI/ML interest

Opportunity:
CSE
1st/2nd year
Python
AI

Result:
94% Match

Also show an explanation:

“Why this opportunity matches you”

with 2–4 reasons.

If a real AI API is not available, implement a transparent rule-based matching algorithm rather than pretending that AI is being used.

Structure the code so a real AI model can be integrated later.

==================================================
9. OPPORTUNITY DETAILS PAGE
==================================================

Clicking an opportunity should open a detailed page.

Include:

- Title
- Organization
- Description
- Eligibility
- Skills required
- Benefits
- Location
- Mode
- Deadline
- Important dates
- Official registration link
- Source
- Verification status
- Last verified date
- Match percentage
- Why it matches the student

Buttons:
[Apply Now]
[Save Opportunity]
[Share]

Clearly display:

✓ Verified

Source:
Official Organization Website

Last verified:
4 Oct 2026

==================================================
10. TRUST AND VERIFICATION
==================================================

This is a core feature.

Every opportunity should have a verification status:

✓ Verified
⚠ Under Review
Community Submitted

Create a verification model.

Verified opportunities should show:
- Verified badge
- Source
- Verification date
- Verified by

Do not claim that an opportunity is officially verified unless it has actually been marked verified in the system.

==================================================
11. SAVE OPPORTUNITIES
==================================================

Students can save opportunities.

Create a “Saved” page.

Sections:

Saved Opportunities
Closing Soon
Recently Saved

Allow users to remove saved opportunities.

==================================================
12. APPLICATION TRACKER
==================================================

Create:

“My Applications”

Students can track:

- Interested
- Saved
- Applied
- Shortlisted
- Selected
- Rejected

Example:

Google Hackathon
Status: Applied
Deadline: 12 Oct
Applied on: 5 Oct

Allow the student to update the status.

==================================================
13. DEADLINE MANAGEMENT
==================================================

Clearly highlight deadlines.

Use badges:

🔴 Deadline Today
🟠 2 Days Left
🟡 7 Days Left
🟢 15 Days Left

Create a “Closing Soon” section.

For the MVP, implement in-app deadline notifications/reminders.

If browser notifications are practical, support them, otherwise create an in-app notification center.

==================================================
14. OPPORTUNITY SUBMISSION
==================================================

Allow students, seniors and clubs to submit opportunities.

Create:

“Submit an Opportunity”

Fields:

- Title
- Organization
- Category
- Description
- Eligibility
- Skills
- Deadline
- Registration URL
- Source URL
- Mode
- Location
- Benefits

After submission:

Status:
“Pending Verification”

Do NOT immediately mark community submissions as verified.

==================================================
15. IMPORTANT WOW FEATURE:
PASTE A FORWARDED MESSAGE
==================================================

Create a feature called:

“Turn a Forward into an Opportunity”

A student can paste a WhatsApp/Telegram message or copied opportunity text.

Example input:

“Microsoft is organizing a student hackathon. Open to college students. Registration closes on 18 October. Register here: ...”

The application should extract structured information:

- Opportunity title
- Organization
- Category
- Eligibility
- Deadline
- Skills
- Registration link

Then show:

“Opportunity detected”

Allow the user to review and submit it.

For the MVP, implement this using rule-based extraction or a mock AI service if no API key is available.

Make the architecture ready for an actual AI API later.

==================================================
16. ROLE-BASED CONTRIBUTION
==================================================

Support these roles conceptually:

STUDENT:
- Discover opportunities
- Save
- Apply
- Track applications
- Submit opportunities

SENIOR:
- Submit opportunities
- Add useful tips

CLUB:
- Publish opportunities/events

FACULTY / COLLEGE CELL:
- Verify opportunities
- Publish official opportunities

ADMIN:
- Review submissions
- Verify/reject opportunities
- Manage users and opportunities

For the MVP, demonstrate role-based access with sample accounts or a simple role selector if full authentication is too complex.

==================================================
17. ADMIN / VERIFICATION DASHBOARD
==================================================

Create an admin dashboard showing:

Pending submissions

Each submission should have:

- Opportunity title
- Submitted by
- Date
- Source
- Status

Actions:

[Review]
[Verify]
[Reject]

Admin should be able to mark an opportunity as verified.

==================================================
18. SAMPLE DATA
==================================================

Populate the application with realistic demo opportunities.

Create at least 15–20 sample opportunities across:

- Hackathons
- Scholarships
- Internships
- Research
- Fellowships
- Coding contests
- Workshops

Use clearly marked DEMO DATA where appropriate.

Do not present invented organizations or deadlines as real verified opportunities.

==================================================
19. NOTIFICATION CENTER
==================================================

Create a notification system showing:

- Deadline approaching
- New matching opportunity
- Saved opportunity closing soon
- Verification result
- Application status update

Example:

🔔 “Your saved opportunity closes in 2 days.”

==================================================
20. MOBILE EXPERIENCE
==================================================

The platform must be highly responsive.

Mobile users should be able to:

- Search
- Filter
- Save
- Apply
- Track applications
- Submit opportunities

Use a bottom navigation on mobile:

Home
Explore
Saved
Applications
Profile

==================================================
21. DATABASE / DATA MODEL
==================================================

If using Supabase, create appropriate tables such as:

users/profiles
opportunities
saved_opportunities
applications
submissions
notifications
verification_records

Opportunity fields should include:

id
title
organization
category
description
eligibility
branches
years
skills
deadline
registration_url
source_url
mode
location
verified
verification_status
verified_at
created_at

Keep the schema clean and scalable.

==================================================
22. DEMO EXPERIENCE
==================================================

The application should be optimized for a hackathon presentation.

Create a smooth demo flow:

1. Open landing page
2. Create student profile
3. Dashboard automatically shows personalized opportunities
4. Show “94% Match”
5. Open an opportunity
6. Show verification information
7. Save it
8. Add it to application tracker
9. Show deadline warning
10. Paste a forwarded WhatsApp-style message
11. Convert it into a structured opportunity
12. Submit it for verification
13. Open admin dashboard
14. Verify the opportunity
15. Show it appearing in the opportunity feed

==================================================
23. UX DETAILS
==================================================

Add:
- Loading states
- Empty states
- Toast notifications
- Confirmation dialogs
- Error handling
- Form validation
- Responsive cards
- Hover states
- Accessible buttons
- Clear typography

Avoid unnecessary animations that make the application slow.

==================================================
24. IMPORTANT DEVELOPMENT RULES
==================================================

Do not build a static mockup.

Build functional interactions wherever possible.

Do not leave major buttons non-functional.

Do not use fake AI claims.

Do not claim external data is verified unless the verification state says so.

Use modular components.

Keep code readable and maintainable.

If a backend/API cannot be configured during development, use a clean local/mock data layer so the complete demo still works.

Make the architecture easy to connect to Supabase and an AI API later.

==================================================
25. FINAL HACKATHON VALUE PROPOSITION
==================================================

The final product should clearly communicate:

“OpportunityHub helps students discover the right opportunities at the right time, from trusted sources, without depending on scattered WhatsApp groups or personal networks.”

The three strongest differentiators should be:

1. Personalized opportunity matching
2. Trust/verification system
3. Deadline + application tracking

The “Turn a Forward into an Opportunity” feature should be presented as the main innovative feature.

Build the complete MVP now with polished UI, working navigation, functional filtering, sample data, matching logic, saving, application tracking, submission flow and verification flow.
