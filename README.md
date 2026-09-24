Pine City Zoo App

A multi-section HTML/CSS website for a fictional zoo, from FNB Week 3. Builds on earlier weeks by introducing a tabbed navigation bar, a reusable "info box" card pattern, animal/place detail pages, a weather forecast table, and a feedback form.

🌐 Site Map
Section	Page(s)	Description
Map	index.html	Homepage — zoo map image
Animals	Animals.html → Elephant.html, Giraffes.html, Koalas.html, Monkey.html, Pandas.html, Lions.html, Gemsbok.html, Gorilla.html, Warthog.html	Animal directory with thumbnail cards linking to full profile pages
Places	Places.html → Amphitheatre.html, Insect house.html, Monkey Trail.html, Wild Things Coffee Shop.html, THE LOST FOREST.html, MO'S PIZZA.html, DINE @THE ZOO.html	Attractions & dining directory with the same card pattern
Weather	Weather.html	Current conditions + 6-day forecast table
Feedback	Feedback.html	Contact form (name, email, message)

Every page shares the same top nav (Animals / Map / Places) and bottom nav (Weather / Feedback), styled via style.css.

📁 Project Structure
Pine-City-Zoo-App/
├── index.html              # Homepage (map)
├── Animals.html            # Animal directory
├── Places.html             # Places/dining directory
├── Weather.html            # Weather forecast
├── Feedback.html           # Feedback form
├── Elephant.html, Giraffes.html, ...   # Individual animal pages
├── Amphitheatre.html, MO'S PIZZA.html, ...  # Individual place pages
├── style.css                # Shared stylesheet
├── logo.png, map.png        # Site graphics
├── *-tn.png                  # Thumbnail images for directory cards
├── *.jpg                     # Full-size animal/place photos
└── README.md
✨ Features Demonstrated
Consistent site-wide navigation (top tabs + bottom tabs) across every page
A reusable "info box" card component (thumbnail + title + blurb + arrow icon) used for both the Animals and Places directories
Detail pages with full descriptive content per animal/place
A data table for the weather forecast, with HTML entities for arrows and degree symbols (&uarr;, &darr;, &deg;)
A basic HTML form (<input>, <textarea>) for user feedback
🚀 How to View

No build tools or server required — this is plain static HTML/CSS.

Clone the repository:
bash
   git clone https://github.com/hitonnie/Pine-City-Zoo-App.git
Open index.html in your browser and navigate from there.
🛠️ Built With
HTML5
CSS3
🔧 Known Issues

A few things worth cleaning up if you revisit this project:

Broken thumbnail images on Animals.html — each <img> tag has a stray .png after the closing quote (e.g. src="elephant-tn.png".png/>), which breaks the image path.
Inconsistent image paths — some pages reference logo.png directly, others reference images/logo.png/images/*.png, but there's no images/ folder in the repo, so those will 404.
Missing page — the Feedback form submits to message-received.html, which doesn't exist in the repo.
Typo — "Sartaday" should be "Saturday" in the weather forecast table.
The feedback form has no action/method or JS handler, so submissions aren't actually processed yet.
📚 Context

Built as part of Week 3 coursework, focused on structuring a larger multi-page site with shared navigation, reusable card layouts, and simple forms.
