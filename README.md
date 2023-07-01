# personal-finance-web-challenge

## Overview

The goal of this exercise is to follow [these requirements](./requirements.md) to build a simple personal finance web app where users will enter a saving goal and monthly deposit will be calculated for them.

## Tech Stack

- Frontend: [React](https://react.dev) + [Mantine](https://mantine.dev)
- Backend: [NestJS](https://nestjs.com)
- Database: [PostgreSQL](https://www.postgresql.org) with [Prisma ORM](https://www.prisma.io)

## Repositories

### This exercise is divided into two repositories: 

- [personal-finance-web-challenge-frontend](https://github.com/elsheraey/personal-finance-web-challenge-frontend)
- [personal-finance-web-challenge-backend](https://github.com/elsheraey/personal-finance-web-challenge-backend)

Please review each repository for running instructions.

**Throughout the codebase, you can find multiple comments showcasing different decisions and potential improvements through out the code. These comments are searchable with the following keys: TODO, OPTIMIZATION, REFACTOR and NOTE.**

## Resources

- [Database Schema](https://github.com/elsheraey/personal-finance-web-challenge-backend/blob/main/prisma/schema.prisma)
- [Authentication Endpoints](https://github.com/elsheraey/personal-finance-web-challenge-backend/blob/main/src/auth/auth.controller.ts)
- [Goals Endpoints](https://github.com/elsheraey/personal-finance-web-challenge-backend/blob/main/src/goals/goals.controller.ts)
- [Initial Thoughts](./initial-thoughts.md)

## Notes, Future-work, and Potential Improvements

- JWT authentication with multiple refresh token is fully implemented in the backend. Yet the frontend axios client still requires a request interceptor to use these refresh tokens upon access token expiration.

- Since this is my first use of Mantine. It was fun as it has similar features to all UI libraries out there. Just note that I tried to restrict myself to follow patterns mentioned in the documentation.

- I ended up using Redux instead of restricting myself to localStorage as [initially thought](./initial-thoughts.md) to make the exercise more complete.

- Pagination, List Virtualization and Caching are all potential optimizations though I thought it would be over-doing it for the sake of this exercise.

- For frontend tests, I showcased multiple use-cases of the React Testing Library though I feel I should've done more in terms of E2E and Visual tests but again, I felt like it would be a huge investment for this exercise.