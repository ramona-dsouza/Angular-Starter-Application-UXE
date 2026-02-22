# Starwars Switch Sides

A single-page web application built with Angular and Bootstrap. The project demonstrates a minimal but complete front-end stack suitable for extension into larger applications.

---

## Overview

Starwars Switch Sides is a lightweight Angular starter that combines Angular (core, router, forms, animations), Angular Material, and Bootstrap into one cohesive UI. The application is structured for clarity and maintainability, with a clear separation between shell, routing, and presentation.

---

## Concept

The app uses a simple thematic frame (choosing sides in a conflict) to drive a small set of views and interactions. This keeps the scope tight while still exercising routing, forms, and responsive layout. The goal is to show a working end-to-end flow without unnecessary domain complexity.

---

## Technical Architecture

- **Framework:** Angular (single-page application with client-side routing)
- **UI layer:** Angular Material (components, theming) and Bootstrap (layout, utilities, CSS variables)
- **Build:** Angular CLI production build; output is static assets (HTML, hashed JS/CSS bundles) suitable for any static host
- **Runtime:** ES modules; polyfills and lazy-loading patterns as provided by the Angular toolchain

The entry point is `index.html`, which loads the compiled application into `<app-root>`. Styles are driven by Bootstrap CSS custom properties and optional Angular Material theming. The architecture assumes a clear boundary between the Angular app and any future backend or API integration.

---

## Interaction Model

- **Navigation:** Handled by the Angular router; route changes update the view without full page reloads.
- **UI feedback:** Uses Angular Material and Bootstrap components for consistent behavior and accessibility.
- **Responsiveness:** Layout and components adapt to viewport size via Bootstrap’s grid and breakpoints.

User actions flow through Angular components and services; state is managed within the application layer rather than via external state libraries in this starter.

---

## Setup

If you have the Angular source (not only the built output):

1. Ensure Node.js and npm are installed.
2. From the project root: `npm install`
3. Run the development server: `ng serve`
4. Open the URL shown in the terminal (typically `http://localhost:4200`).

If this repository contains only the production build (e.g. `index.html` and hashed JS/CSS files), serve the root directory with any static file server (e.g. `npx serve`, or deploy to a static host) and open the root URL.

---

## Purpose

This project serves as a portfolio piece and a reusable starter: it shows competency in Angular, Bootstrap, and modern front-end structure without relying on heavy backend or tooling. It is intended to be read and extended by developers who care about clean structure, systems thinking, and pragmatic technical choices in web applications.
