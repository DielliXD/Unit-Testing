# Angular Unit Testing

A small Angular 17 app built to practice unit testing. Each component, page and service has its own spec file.

## What is tested

- **Reusable components:** `Button` and `Link` with different variants, types and router links, tested through a host component
- **Contact page:** reactive form renders all fields, and the submit button stays disabled until the form is valid
- **Home page:** loads a user list through `UserService`, with the service mocked so no real HTTP calls are made
- **UserService:** HTTP requests tested with `HttpClientTestingModule`
- **Component logic:** properties, methods and rendered DOM elements

## Tech stack

- Angular 17 (standalone components), TypeScript
- Jasmine and Karma
- Tailwind CSS
- Reactive Forms, Angular Router, HttpClient

## Project structure

    src/app/
      component/   reusable UI (button, link, about, my-component)
      page/        home, contact
      service/     user.service
      interface/   TypeScript models
      mock/        test data

## Run locally

    npm install
    npm start      # app on http://localhost:4200
    npm test       # run unit tests
