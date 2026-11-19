# AlphaRoom — Hotel Room Booking Application

AlphaRoom is a MERN-stack learning project for exploring a hotel room discovery and reservation workflow. It includes a React client and an Express/MongoDB backend.

> **Project context:** This is an independent learning project, not a customer production system.

## Overview

The application demonstrates a typical hotel booking journey: users can explore available rooms, review room details, make reservations, and manage their bookings. It also includes administrative functionality for managing rooms and booking-related records.

## Key features

- Browse and view hotel rooms.
- Search and filter rooms using booking-related criteria.
- Register and sign in to the application.
- Create room reservations and review booking costs.
- View booking history and manage/cancel reservations.
- Administrative views for managing rooms, users, and bookings.
- Stripe test-mode checkout integration.

Payment integration is documented as a test-mode implementation; it should not be treated as a live payment service.

## Technology stack

| Area | Technologies |
|---|---|
| Frontend | React, React Router |
| UI | Ant Design, React Bootstrap, Bootstrap |
| Backend | Node.js, Express |
| Database | MongoDB, Mongoose |
| HTTP requests | Axios |
| Payments | Stripe test integration |
| Utilities | Moment.js, SweetAlert2 |

## Repository structure

The repository separates the React client from the server-side application:

- `client/` — React frontend
- Root-level server files and configuration — Express backend and related dependencies

## Run locally

### Prerequisites

- Node.js and npm
- A MongoDB database
- Stripe test credentials if testing the checkout flow

### Install dependencies

Install the backend dependencies from the repository root:

```bash
npm install
```

Install the frontend dependencies:

```bash
cd client
npm install
```

### Configure environment

Configure the database connection, authentication settings, and Stripe test credentials wherever they are read by the server and client. Use test credentials only, and do not commit secrets to the repository.

### Start the application

Start the backend using the server entry point and startup configuration present in the repository. Then, in a separate terminal, start the React client:

```bash
cd client
npm start
```

The frontend development server is provided by Create React App. The backend start command may depend on the server entry file and local environment configuration.

## What this project demonstrates

AlphaRoom was an early hands-on project for learning full-stack application development. It helped me practice connecting a React interface to an Express API, working with MongoDB models, implementing booking-related workflows, and integrating a payment provider in test mode.

## Security and production note

This repository is a learning project and should not be assumed to be production-ready. Review authentication, authorization, input validation, payment handling, environment configuration, and dependency versions before deploying it or processing real payments.
