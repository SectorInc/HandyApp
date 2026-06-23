# HandyApp

HandyApp is a static website for finding verified handymen for services such as plumbing, painting, cleaning, carpentry, tiling, electrical work, and satellite dish installation.

The site is currently built with plain HTML and CSS. It does not require a backend server, database, or build tool to preview.

## Pages

- `handyapp.html` - Home page and main landing page.
- `join.html` - Join page for customers and handymen.
- `services.html` - Service listing page with booking buttons.
- `handyapp-signIn.html` - Sign-in page.
- `handyman-signUp.html` - Sign-up page.
- `news.html` - Latest news and updates page.

## Stylesheets

- `handyapp.css` - Home page styling.
- `join.css` - Join page styling.
- `services.css` - Services page styling.
- `handyapp-signIn.css` - Sign-in page styling.
- `handyapp-signUp.css` - Sign-up page styling.
- `news.css` - News page styling.

## Assets

Images are stored in the `IMG` folder. The HTML files reference these images directly, so keep the folder name and file paths unchanged unless you also update the matching HTML.

## How To Run

Open `handyapp.html` directly in a browser, or run a simple local server from the project folder.

Example with Python:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000/handyapp.html
```

## Current Form Flow

Because this is a static website, the forms use `method="get"` and navigate between existing HTML pages.

- Home email form sends users to `handyman-signUp.html`.
- Sign-up form sends users to `handyapp-signIn.html`.
- Sign-in form sends users to `services.html`.
- Service booking buttons send users to `handyapp-signIn.html` with the selected service included as a query value.

This avoids `405 Method Not Allowed` errors that happen when a static HTML page receives a `POST` request without a backend server.

## Future Improvements

- Add backend authentication for real sign-up and sign-in.
- Store user accounts and bookings in a database.
- Add booking confirmation pages.
- Display selected service details after sign-in.
- Improve form validation and accessibility labels.
- Add mobile navigation for smaller screens.

## Project Status

This is an early static prototype of the HandyApp website. It is ready for browser preview and continued frontend development.
