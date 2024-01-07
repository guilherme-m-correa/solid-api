# Solid API - Node.js

A GymPass-Style App using the principles of SOLID

## Technologies

- Fastify
- Typescript
- PrismaORM
- PostgreSQL
- Vitest
- Zod

### Functional Requirements

- **User Registration:**
  - Users should be able to register.

- **Authentication:**
  - Users should be able to authenticate.

- **User Profile:**
  - Users should be able to retrieve the profile of a logged-in user.

- **Check-in Count:**
  - Users should be able to obtain the number of check-ins performed by the logged-in user.

- **Check-in History:**
  - Users should be able to view their check-in history.

- **Nearby Gyms:**
  - Users should be able to search for gyms within a 10km radius.

- **Search Gyms by Name:**
  - Users should be able to search for gyms by name.

- **Check-in at a Gym:**
  - Users should be able to check in at a gym.

- **Validate User's Check-in:**
  - Users' check-ins should be validated.

- **Register Gym:**
  - Admins should be able to register a gym.

### Business Rules

- **Unique Email Registration:**
  - Users cannot register with a duplicated email.

- **Daily Check-in Limit:**
  - Users cannot perform more than one check-in in a single day.

- **Proximity Check:**
  - Users cannot check in unless within 100m of the gym.

- **Check-in Validation Time Limit:**
  - Check-ins can only be validated within 20 minutes of creation.

- **Admin Validation:**
  - Check-ins can only be validated by administrators.

- **Admin-Only Gym Registration:**
  - Gym registration can only be performed by administrators.

### Non-Functional Requirements 

- **Encrypted User Password:**
  - User passwords must be encrypted.

- **Data Persistence:**
  - Application data must be persisted in a PostgreSQL database.

- **Paginated Data Lists:**
  - All data lists must be paginated, with 20 items per page.

- **User Identification with JWT:**
  - Users should be identified using JSON Web Tokens (JWT).
