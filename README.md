# MLH-Events
A website which scrapes the [MLH Events](https://mlh.io/events) page and display all the events in the website.

### Live Wesbite:
The live website can be viewed via multiple links:
- GitHub Pages: [https://rajatshenoi.github.io/MLH-Events](https://rajatshenoi.github.io/MLH-Events/)
- My Personal Website: [https://old.rajatshenoi.live/MLH-Events/](https://old.rajatshenoi.live/MLH-Events/)
- Repl.it: [https://mlh-events.rajatshenoi.repl.co/](https://mlh-events.rajatshenoi.repl.co/)

### Stuff Used:
- **Replit**: Coded the entire website using [Repl.it](https://repl.it/) with the help of [MLH](https://mlh.io/) at the [Global Hack Week: Data](https://ghw.mlh.io/).
- **MLH Events Page**: [this](https://mlh.io/events) is the page that the script scrapes and stores data from which is then rendered on my version of the website.
- **Google Apps Script:** the backend of the website is over [here](https://script.google.com/home).
  - **GetEventsEndpoint.gs:** API which retrieves data from the database, in this case, [Google Sheets: MLH Events](https://docs.google.com/spreadsheets/d/1r35ZClUg9f78wnwE0Denfz83W3K460AofJKGBrbcvAs/edit?usp=sharing) and returns the data in JSON format.
  - **ScrapeMLHEvents.gs:** Uses the [Cheerio library](https://github.com/tani/cheeriogs) to scrape the MLH Events page and load that data into the above mentioned Google Sheet.
  - **Triggers:** Configured Google Apps Scripts to execute the **ScrapeMLHEvents** function everyday between **Midnight and 1am** Indian Standard Time thereby keeping the Google Sheet (database) up to date with the latest events.
- **Trailwind CSS:** [this](https://tailwindcss.com/) was library used to style the website.
- **daisyUI:** [this](https://daisyui.com/) was the library used to make use of the Trailwind CSS library very easily.
- **Cheerio:** is the [website scraping tool](https://cheerio.js.org/) that was used in this project to scrape MLH's website.
