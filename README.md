<h1 align="center">Hi 👋, I'm @BenjaminTietz</h1> <h3 align="center">A passionate fullstack developer from Germany.</h3> <p align="center"> <img alt="Coding GIF" width="300px" height="auto" src="https://github.com/user-attachments/assets/f72af3a4-5aa0-4c11-9bf3-eeeab6c87b23"/> </p> I'm currently working on 🛠

## 🇹🇭 Thailand Vloggers Platform

A large-scale **creator discovery platform for Thailand travel
YouTubers**.

The project is designed as a **modern headless architecture** combining
a high-performance static website, a creator dashboard, and a scalable
backend system.

The goal of the platform is to connect:

-   Thailand travel creators
-   travel destinations
-   travel guides
-   video content

into a **structured SEO-driven content ecosystem**.

------------------------------------------------------------------------

## 🏗 Platform Architecture

The system follows a **three-layer architecture**.

    Static SEO Platform (SSG)
            │
            ▼
    Creator Dashboard (CSR)
            │
            ▼
    Django REST Backend

------------------------------------------------------------------------

### 1️⃣ Public Website --- Static Site Generation

The public website is built with **Angular** and prerendered using
**SSG**.

Goals:

-   Maximum SEO performance
-   Extremely fast load times
-   Highly scalable content structure

Features:

-   Creator profiles
-   Region hubs
-   Category hubs
-   Travel guides
-   YouTube video integration
-   Topic cluster SEO architecture

All content is stored as structured JSON files.

Example:

    src/content/creators/*.json
    src/content/regions/*.json
    src/content/categories/*.json
    src/content/guides/*.json

This allows the platform to scale to **hundreds of creators and
thousands of pages** while maintaining performance.

------------------------------------------------------------------------

### 2️⃣ Creator Dashboard --- Angular Application

The platform also includes a **separate Angular dashboard** where
creators can manage their profiles.

Features:

-   Creator account system
-   Profile editing
-   Social links management
-   Media uploads
-   Change request workflow
-   Notifications

Architecture:

-   Angular SPA
-   JWT Authentication
-   REST API communication with Django backend

Creators **do not modify live content directly**.

Instead they submit **change requests** which are reviewed before going
live.

------------------------------------------------------------------------

### 3️⃣ Backend --- Django REST Platform

The backend is built with:

-   Python
-   Django
-   Django REST Framework
-   PostgreSQL

Responsibilities:

-   Authentication system
-   Creator profile management
-   Moderation workflows
-   Media upload pipeline
-   Community features
-   Content synchronization

The backend acts as the **single source of truth** for creator data.

Approved content can be exported to JSON files which are used by the
static site.

------------------------------------------------------------------------

## 🔄 Content Synchronization Pipeline

The platform combines **database-driven editing** with **static site
performance**.

    Creator submits change
            │
    Admin approves change
            │
    Database updated
            │
    Content exported to JSON
            │
    GitHub Action triggers rebuild
            │
    Static site redeployed

This allows **fast, SEO-optimized pages** while still supporting
**dynamic content management**.

------------------------------------------------------------------------

## 💻 Tech Stack

Frontend

-   Angular
-   TypeScript
-   RxJS
-   SCSS

Backend

-   Python
-   Django
-   Django REST Framework
-   PostgreSQL

Infrastructure

-   Docker
-   Nginx
-   Apache
-   GitHub Actions

------------------------------------------------------------------------


## 👨‍💻 Portfolio

Some of my projects are available at:

🔗 https://benjamin-tietz.com

------------------------------------------------------------------------

## 📫 Contact

mail@benjamin-tietz.com

------------------------------------------------------------------------

## 💻 Tech Stack

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Angular](https://img.shields.io/badge/angular.js-%23E23237.svg?style=for-the-badge&logo=angularjs&logoColor=white)
![Django](https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white)
![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![RxJS](https://img.shields.io/badge/rxjs-%23B7178C.svg?style=for-the-badge&logo=reactivex&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)

