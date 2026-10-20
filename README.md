# Kino's Travel Guide: Travel Japan

> A multi-page travel website for exploring Japan: destination guides, trip-planning tools, and local-style tips for travelers.

---

## About

Kino's Travel Guide aims to be "your friend in Japan, guiding you like a local". The site highlights must-see destinations from Tokyo to Kyoto and Osaka, and helps visitors plan their trip with a checklist, itineraries, and travel packages.

## Features

- **Hero carousel**: full-screen slides introducing the guide, iconic spots, culture, and trip planning
- **Popular Places**: photo cards that open quick-view modals with a short description and a "Read More" link
- **Destination pages**: a dedicated page for each landmark
- **Trip planning tools**: travel checklist, itinerary, and package/trip planning pages
- **Live search**: type in the navbar to get destination suggestions as you go
- **Traveler testimonials**: a "What Our Travelers Say" section
- **Responsive design**: sticky, collapsible navbar and mobile-friendly layout

## Destinations

| Destination                     | Location | Page                  |
| ------------------------------- | -------- | --------------------- |
| Kuromon Ichiba Market           | Osaka    | `kuromon.html`        |
| Osaka Castle                    | Osaka    | `osakacastle.html`    |
| Arashiyama Bamboo Grove         | Kyoto    | `bamboogrove.html`    |
| Arashiyama Monkey Park          | Kyoto    | `arashiyama.html`     |
| Matsumoto Castle                | Nagano   | `matsumoto.html`      |
| Shinjuku Gyoen National Garden  | Tokyo    | `shinjukugyoen.html`  |
| Tokyo Imperial Palace           | Tokyo    | `imperial.html`       |
| Mount Fuji                      | Honshu   | `mountfuji.html`      |

## Tech Stack

- HTML5, CSS3, and vanilla JavaScript
- [Bootstrap 5.3.5](https://getbootstrap.com/) (via CDN)
- [Bootstrap Icons 1.11.1](https://icons.getbootstrap.com/) (via CDN)

## Project Structure

```
Travel-Guide/
├── index.html            # Home: carousel, popular places, testimonials, search
├── destination.html      # All destinations
├── travelchecklist.html  # Trip planning: checklist
├── itinerary.html        # Trip planning: itinerary
├── package.html          # Trip planning: packages
├── kuromon.html          # Destination detail pages
├── bamboogrove.html
├── arashiyama.html
├── matsumoto.html
├── shinjukugyoen.html
├── osakacastle.html
├── imperial.html
├── mountfuji.html
├── Images/               # Photos and logos
└── README.md
```

## Getting Started

No build step is required.

1. **Clone the repository**
   ```bash
   git clone https://github.com/HiraiGinji/Travel-Guide.git
   cd Travel-Guide
   ```

2. **Open the site**
   - Double-click `index.html`, **or**
   - Serve it locally:
     ```bash
     python -m http.server 8000
     ```
     Then visit `http://localhost:8000`.

> An internet connection is needed for the Bootstrap and Bootstrap Icons CDNs.

## Adding a New Destination

1. Create a new page, for example `newplace.html`, based on an existing destination page.
2. Add the image to `Images/`.
3. Add a card and modal to the Popular Places section in `index.html`.
4. Add an entry to the `destinations` array in the search script:
   ```js
   { name: "New Place", link: "newplace.html" }
   ```

## Author

Created by [HiraiGinji](https://github.com/HiraiGinji).
