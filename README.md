# ScotJam website

Public pages for ScotJam, Scouts Scotland’s national summer camps.  The site is plain HTML and CSS.  There is no build step and nothing to compile.

## Pages

| Menu label | Page | File |
| --- | --- | --- |
| Home | ScotJam | `index.html` |
| Activities | Activities and programme | `activities.html` |
| Info | Info for leaders and parents | `info.html` |
| Volunteer | Volunteer with us | `volunteer.html` |
| Contact | FAQs and contact | `contact.html` |

There is no booking or fees page, and no Meet the Team page.

## How to edit a page

You can do this on the GitHub website.  You do not need to install anything.

1. Open this repository on GitHub.
2. Click the page you want, for example `info.html`.
3. Click the pencil icon (Edit this file).
4. Change the sentences inside `<main>`.  Leave the words in angle brackets as they are.  Those tags are the structure of the page.
5. After a full stop, type two spaces, then the next sentence.  Keep each paragraph on one line.  The stylesheet is set up so those two spaces stay visible.
6. Commit the change to the `main` branch.

Search a file for `TO CONFIRM` before you add a new fact.  [TO-CONFIRM.md](TO-CONFIRM.md) lists every one, with the file it is in.  On the public page, leave a normal sentence such as “More details coming soon” until you know the answer.  Do not put the words `[TO CONFIRM]` on the page.

If you change the menu or the footer, make the same change in every HTML file, including `404.html`.  The footer must keep this line: ScotJam is a Scouts Scotland event.  Scouts Scotland is a registered Scottish Charity No. SC017511.

The only public email address is [scotjam@scouts.scot](mailto:scotjam@scouts.scot).  Do not add personal email addresses, phone numbers, a form that collects children’s details, or fees.

Photographs: do not add photos of young people unless you have media consent for this website.  Each empty photo box has an HTML comment just above it with suggested alt text.

The header logo is an empty slot, with the word ScotJam beside it.  See [assets/logo/README.md](assets/logo/README.md) for how to drop in the official Scouts Scotland logo from the brand centre.  Do not draw the fleur-de-lis yourself.

Colours and the font are set in `css/custom.css`.  The pages also load [Scoutstrap](https://scoutstrap.github.io/) (a Scouts theme for Bootstrap 4) and Nunito Sans from the links in each page.  Scoutstrap’s purple and teal are out of date, so `custom.css` replaces them with the current Scouts palette from brand guidelines v3.3 (August 2026): Scouts Purple `#7413dc`, Scouts Blue `#006ddf`, Teal `#088486`, Navy `#003982`, and the other colours listed at the top of that file.  Headings use Nunito Sans Black.  The word ScotJam in the header uses Extra Bold.  Body text uses Regular.

## Turn on GitHub Pages

The site is ready to publish from the root of the `main` branch.  `index.html` is in the root.  The empty `.nojekyll` file tells GitHub not to run Jekyll.

1. In this repository, open **Settings**.
2. Open **Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Branch: **main**.  Folder: **/ (root)**.
5. Save.

After a short wait, GitHub shows the site address.  It will look like `https://eoin-scouts.github.io/scotjam-website/`.

A later edit on `main` updates the live site after GitHub republishes it.

## scotjam.co.uk, later

Do not connect scotjam.co.uk yet.  There is no `CNAME` file, on purpose.  Leave the domain on the current site until you approve the switch.

When you are ready:

1. Add the custom domain in **Settings > Pages**.
2. Add a `CNAME` file in the root of `main` containing only `scotjam.co.uk`.
3. Change the DNS for scotjam.co.uk with whoever looks after the domain, so the current site is not switched off by accident.

GitHub’s Pages documentation explains the DNS records.  Do that only after you have approved the move.

## Facts already confirmed

- Beavers: 4 to 6 June 2027
- Scouts: 10 to 17 July 2027
- Cubs: 19 to 23 July 2027
- Explorers: 25 to 31 July 2027
- Sections: Beavers, Cubs, Scouts and Explorers
- Booking opens: to be confirmed
- Public contact: scotjam@scouts.scot only
- Charity: SC017511
