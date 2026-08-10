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
