![NextJS](https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#overview">Overview</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
        <li><a href="#demo">Demo</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li>
      <a href="#features">Features</a>
      <ul>
        <li><a href="#user-experience">User Experience</a></li>
        <li><a href="#performance">Performance</a></li>
      </ul>
    </li>
    <li><a href="#design">Design</a></li>
    <li><a href="#branding">Branding</a></li>
    <li><a href="#accessibility--optimisation">Accessibility / Optimisation</a></li>
    <li><a href="#contributions">Contributions</a></li>
    <li><a href="#scaling--future-enhancements">Scaling & Future Enhancements</a></li>
    <li><a href="#credits">Credits</a></li>
  </ol>
</details>

# Overview

**PathSnap** is a full-stack link shortening web application. PathSnap was created with ease of use, speed, and style in mind. A strong backend and a slick interface make it simple to create, manage, and distribute shortened links.

## Built With

**Frontend**

- Next.js (App Router)
- TailwindCSS
- TypeScript

**Backend**

- Laravel
- MySQL

**Hosting**

- Frontend deployed on Vercel with CI/CD.
- Backend deployable on any LAMP/VPS/Forge setup.

## Images

![Home Page](https://i.imgur.com/lNNRDGX.jpeg)
![Links Page](https://i.imgur.com/WHnRuEb.jpeg)

# Getting Started

To get started with PathSnap locally, ensure all prerequisites are met and follow the installation guide.

## Prerequisites

```bash
# Download and install nvm:
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.1/install.sh | bash
nvm install 22
nvm use 22

# Check versions
node -v     # Should print v22.x
npm -v      # Should print >=10.x
php -v      # PHP >= 8.2
composer -V # Composer installed
mysql       # Installed and running
```

## Installation

### 1. Clone the repositories

```bash
git clone https://github.com/psyofrelief/pathsnap-frontend.git
git clone https://github.com/psyofrelief/pathsnap-backend.git
```

### 2. Setup the frontend

```bash
cd PathSnap-frontend
cp .env.example .env.local
npm install
npm run dev
```

### 3. Setup the backend

```bash
cd ../PathSnap-backend
cp .env.example .env
composer install
php artisan key:generate
php artisan migrate
php artisan serve
```

> Make sure your backend `.env` is configured correctly with your DB connection and CORS settings for your frontend.

# Features

## User Experience

- Mobile-first responsive design.
- Intuitive UI with modals for creating and editing links.
- QR code generator & shortlink copy-to-clipboard functionality.

## Performance

- Optimised loading with suspense boundaries.
- Loading indicators and overlays.
- Server-side rendering.

# Design

### Design Philosophy:

- Simplicity-first UI with focus on readability and usability.
- Inspired by tools like Bitly, Linktree with original visual identity.

### Tech Highlights:

- Utility-first CSS via Tailwind.
- Scoped reusable components with best practices.

# Branding

**PathSnap** stands for _Pretty Zippy And Good_ — a quick, entertaining, and practical tool to speed link exchange.

# Accessibility / Optimisation

- High contrast themes and semantic HTML.
- ARIA roles for modals and buttons.
- Lighthouse-tested performance & accessibility scores.
- Optimised backend routes with JSON:API conventions.

# Contributions

This project is private and solely maintained by [Faried Idris](https://faried.vercel.app).

# Scaling & Future Enhancements

- Rate limiting / spam protection.
- Scheduled link expiration & redirection rules.
- Analytics dashboard.

# Credits

Developed and designed by **Faried Idris**.
For inquiries, visit [faried.vercel.app](https://faried.vercel.app) or connect on GitHub / LinkedIn.

```

```
