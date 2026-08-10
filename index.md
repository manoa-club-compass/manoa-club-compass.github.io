# Mānoa Club Compass

[![Club Compass CI](https://github.com/manoa-club-compass/manoa-club-compass-nextjs/actions/workflows/ci.yml/badge.svg)](https://github.com/manoa-club-compass/manoa-club-compass-nextjs/actions/workflows/ci.yml)

## Overview

Mānoa Club Compass is a centralized directory for UH Mānoa student organizations. It helps students discover clubs, browse by interest area, and find meeting and contact information.

## GitHub Organization and Repositories

- [Mānoa Club Compass organization](https://github.com/manoa-club-compass)
- [Next.js application repository](https://github.com/manoa-club-compass/manoa-club-compass-nextjs)
- [Project home repository](https://github.com/manoa-club-compass/manoa-club-compass.github.io)

## Club Compass Scope

- Students can browse and filter clubs by interest area.
- Students can view club descriptions, categories, contacts, and websites.
- Club administrators can update their club profile.
- Super Admins can review club profiles and save approval or rejection decisions.

## Team Contract

[View our Team Contract](https://docs.google.com/document/d/1Awi8W8y4iuA7VAnEgqY_-I3zPHUNi6GED164ORaw-MU/edit?tab=t.0)

## Deployment

[Open Mānoa Club Compass on Vercel](https://manoa-club-compass-nextjs.vercel.app/)

## Milestones
 
### Milestone 1

[View the M1 Project page](https://github.com/orgs/manoa-club-compass/projects/2)
  
### Milestone 2

[View the M2 Project page](https://github.com/orgs/manoa-club-compass/projects/3)

### Milestone 3 
[View the M3 Project page](https://github.com/orgs/manoa-club-compass/projects/4)

## User Guide

### Landing Page

![Landing-page recent](images/landing-page.png)

The landing page introduces Mānoa Club Compass. Select **Browse clubs** to explore the directory without signing in, or use the navigation menu to sign in or create an account.

### Accounts and Role Access

Select **Sign up** to create a student account with an email address and password. Returning users can select **Sign in** and enter their credentials. After signing in, use the account menu to sign out. Club Admin and Super Admin navigation options appear only for accounts with those roles.

### Browse Clubs

![Browse-clubs recent](images/browse-clubs.png)

Use the search box to find clubs by name, description, or interest area. Use the category menu to narrow the directory. Select **View details** on any result to open its full profile.

### Club Details

![Club-details recent](images/club-details.png)

The Club Details page displays the organization’s description, interest area, website, and contact information when those details are available. Use the listed website or email address to contact the organization.

### Club Admin Dashboard

![Club-admin recent](images/club-admin.png)

Club Admins can open **Club admin** after signing in. They can create or update their organization’s name, description, interest area, website, and contact email. Select **Create club** or **Save changes** to store the profile in the directory.

Regular student accounts cannot open the Club Admin or Admin Dashboard pages.

### Super Admin Dashboard

![Current Super Admin review queue](images/admin-dashboard.png)

Super Admins can open **Admin dashboard** to review every club profile. Each row shows the club’s category and saved review status. Select **Approve** or **Reject** to record a decision. The status badge updates after the action and remains saved after the page is reloaded.

## Community Feedback

Five UH community members outside ICS 314 tested the deployed application on mobile and desktop devices. To protect their privacy, the findings below are reported in aggregate without names, affiliations, devices, test dates, or individual quotations.

Testers completed the same short workflow: identify the application’s purpose, browse the club directory, search for an interest, filter by category, open a club profile, and describe what worked and what should improve. Their average usefulness rating was **3.4 out of 5**.

### What worked well

- The application’s purpose and primary navigation were immediately understandable.
- Search, category filtering, and club cards were simple to use.
- The responsive layout remained readable on smaller screens and at increased zoom levels.
- Searching description text helped testers discover relevant clubs beyond exact name matches.

### What needs improvement

- Club profiles need more complete and current information, especially meeting times, locations, verification status, and last-updated dates.
- Search and filter choices should be reflected in the URL, and result counts would make filtered views easier to understand and share.
- Club names should appear in page headings and browser tab titles for clearer navigation and better screen-reader support.
- Loading failures, empty searches, and missing club pages need clear recovery actions instead of dead ends or misleading empty states.
- Club officers need a clearer path to claim and maintain their organization’s listing.

### Team response

Milestone 3 added a Super Admin review workflow that records approval and rejection decisions. The feedback shows that the public directory must also communicate verification clearly and avoid exposing incomplete or test records. Meeting details, shareable filter URLs, page metadata and heading improvements, resilient error states, and a club-claim workflow are documented as priorities for future development. These findings are based on the five testers’ actual responses; no participant feedback was generated or inferred by the team.

## Developer Guide
 
1. **Install PostgreSQL** and create a database:
```
createdb manoa-club-compass
```
 
2. Clone the repo on Github.
  
3. Install dependencies:
```
npm install
```
 
4. Create your `.env` file — copy `sample.env` to `.env` and update `DATABASE_URL`.
  
5. Run migrations:
```
npx prisma migrate dev
```
 
6. Generate the Prisma client:
```
npx prisma generate
```
 
7. Seed the database:
```
npm run seed
```
 
8. Start the dev server:
```
npm run dev
```
 
The app should run at http://localhost:3000.

 
## M1 Page  Mockups

The following show the M1 required supporting-page mockups.

### Landing Page Mockup

![Landing-page mockup](images/landing-page-mockup.png)

### Browse Clubs Mockup

![Browse-clubs mockup](images/browse-clubs-mockup.png)

### Club Details Mockup

![Club-details mockup](images/club-details-mockup.png)

### Club Admin Dashboard Mockup

![Club-admin mockup](images/club-admin-mockup.png)


### Admin Dashboard Mockup

![Admin mockup](images/admin-dashboard-mockup.png)
