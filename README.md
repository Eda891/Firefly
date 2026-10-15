# Firefly Cinema 🎬

**A small room. A big picture.**

Firefly Cinema is a responsive, single-screen independent cinema website concept. It showcases a weekly film programme and includes an interactive seat-selection and reservation experience.

🌐 **Live website:** https://fireflycinema.netlify.app/

## Features

- **Cinema landing page** — a hero section, cinema details, and clear booking links.
- **Now Showing** — film cards with custom CSS poster artwork, genres, descriptions, and screening times.
- **Interactive seat map** — a 5-row layout (A–E) with 6 seats per row.
- **Screening selection** — choose from the available film screenings.
- **Seat selection** — select available seats, choose a random seat, and reserve up to six seats at a time.
- **Booking confirmation** — view a ticket-style confirmation with the selected screening and seats.
- **My Reservations** — look up reservations by email and cancel bookings.
- **Contact form UI** — a client-side demo form with a confirmation message.
- **Responsive layout** — adapts the layout for smaller screens.
- **Local persistence** — reservations and seeded seat availability are saved in the browser using `localStorage`.

## Films Featured

The current demo programme includes:

- **The Hollow Choir** — Horror, Supernatural, Thriller
- **Sprocket & the Star Machine** — Animation, Comedy, Adventure, Family
- **Meridian** — Adventure, Action, Fantasy

These titles and their poster designs are fictional demo content.

## Tech Stack

- **HTML5** — page structure and content
- **CSS3** — styling, responsive layout, gradients, and poster artwork
- **Vanilla JavaScript** — seat selection, booking interactions, reservation lookup, and cancellation
- **Web fonts** — Big Shoulders Display, Work Sans, and Space Mono via Google Fonts
- **Browser `localStorage`** — local demo data persistence
- **Netlify** — live hosting

No frontend framework, package manager, or build step is required for the current single-file implementation.

## Getting Started

### View the live website

Visit: https://fireflycinema.netlify.app/

### Run locally

1. Download or clone this repository.
2. Ensure the main HTML file is named `index.html`.
3. Open `index.html` in a modern web browser.

Alternatively, use a local development server, such as the **Live Server** extension in Visual Studio Code.

## How the Reservation Demo Works

1. Enter a name and email address.
2. Select a screening.
3. Choose available seats from the seat map, or use **Pick a random seat**.
4. Select **Confirm booking**.
5. View the ticket-style confirmation.
6. Open **My Reservations**, enter the same email address, and find or cancel reservations.

The demo supports up to six seats selected at once. Reservations are stored in the current browser's `localStorage`.

## Important Limitations

This project is currently a **frontend demo**, not a production-ready ticketing system.

- **Browser-local storage:** reservations are stored only in the browser where they were created. They are not shared between devices, browsers, or visitors.
- **No central inventory:** seat availability is not synchronized through a backend, so simultaneous users cannot reliably reserve seats without conflicts.
- **No payment processing:** the site does not collect payment or issue paid tickets.
- **Contact form:** the form displays a demo confirmation message but does not send messages. Connect it to a service such as Netlify Forms, Formspree, or a custom backend to receive submissions.
- **Demo seat availability:** some seats are randomly marked as taken on first use for each screening, and that initial layout is saved locally.
- **Demo content:** film listings, venue details, and contact information are sample content. Verify and replace them before using the site for a real cinema.

**Privacy note:** avoid entering real personal information into the demo. Names and email addresses associated with bookings are stored in the browser's local storage.

## Project Structure

```text
.
└── index.html   # HTML markup, CSS styles, and JavaScript interactions
```

## Deployment

The site is hosted on Netlify.

For a simple static deployment:

1. Make sure `index.html` is at the published site's root.
2. Deploy the file or connect the repository to Netlify.
3. For this single-file version, no build command is needed; publish the directory containing `index.html`.

After deploying changes, open the live URL and test the booking, reservation lookup, cancellation, and contact form behavior.

## Future Improvements

- Add a backend and database for shared, reliable reservations.
- Prevent double-booking with server-side seat validation.
- Add secure booking confirmation emails.
- Connect the contact form to an email or form-processing service.
- Add payment integration if paid tickets are required.
- Replace demo listings and contact details with verified production information.
- Add automated tests and accessibility checks.

## License

No license is specified yet. Add a `LICENSE` file if you intend to make the project open source, and choose a license that fits how you want others to use it.

---

Made for people who love the big screen and the small cinema experience. 🍿
