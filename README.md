# VoyageVista - Travel Booking Platform

A multi-page travel booking website that extends the Travel Deals concept with a Node.js/Express backend. VoyageVista lets users search flights and hotel stays, manage separate booking carts, register and log in, and submit contact enquiries. Flight and hotel data are stored in XML and JSON files respectively; contact submissions are written to an XML file server-side.

## Key Features

- **Flight Search** - Search one-way or round-trip flights by origin, destination, departure/return date, and passenger count; the backend reads from flights.xml and returns matching results
- **Hotel Stays Search** - Browse available hotel accommodations sourced from hotels.json
- **Separate Booking Carts** - Independent cart pages for flights and hotel stays, each persisted in JSON files (cart.json and cartHotel data)
- **Booking History** - Dedicated history pages for past flight and hotel reservations
- **User Registration and Login** - Account creation and login pages with dedicated CSS styling
- **Contact Us Form** - Form submissions are validated and saved to contacts.xml via an Express POST endpoint
- **Accessibility Controls** - Font size and background color controls on every page (Normal/Large/Extra Large and White/Gray/Black)

## Tech Stack

| Layer | Technologies |
|---|---|
| Frontend | HTML5, CSS3, JavaScript (jQuery, AJAX) |
| Backend | Node.js, Express.js |
| Data Parsing | xml2js (XML parsing), fs (file I/O) |
| Data Storage | XML (flights, contacts, bookings), JSON (hotels, carts) |
| Middleware | body-parser, cors |
| Icons | Font Awesome 6 |

## Setup and Installation

Prerequisites: Node.js 18+ installed locally.

1. Clone the repository:
   ```bash
   git clone https://github.com/moksh555/VoyageVista.git
   cd VoyageVista
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the Express server:
   ```bash
   node server.js
   ```
4. Open http://localhost:3000 in your browser.

## Usage

- Open index.html (served by Express) to reach the home page
- Navigate to **Flights** to search for available flights by route and date
- Navigate to **Stays** to browse hotel options
- Add items to your **Flight Cart** or **Hotel Cart** and review before booking
- Register or log in via the **Register** and **Login** pages
- Submit enquiries via the **Contact Us** form
