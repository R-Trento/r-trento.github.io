# R-Trento Users Group website

The site is built with Quarto and it is supposed to be published on GitHub pages.

## How to build the site

From the terminal, run the following command to get a local preview:

```bash
quarto preview
```

To build the site, run the following command:

```bash
quarto publish gh-pages
```

## How to contribute

### Posts

To create a new post, look into the `posts` folder, duplicate the `000-template` folder and give it a name starting with an incremental number ( e.g. `123-new_post`). Then, edit the `index.md` file with your content and add an illustrative image. Hint: use <https://recraft.io> to generate an image.

When editing the `index.md` file, remember to update the YAML preamble:

- Set a proper title
- Set the author (your name, preverably)
- Set the date (MM/DD/YYYY)
- Set the image (the name of the image file)
- Give a list of categories (e.g. `RTUG`, `milestone`, `R`, `tidyverse`, etc.)

Once you are done, **remember** to set `draft: false` in the YAML preamble.

### Meetings announcements

Similarly to the posts, you can create a new meeting announcement by creating a new `.qmd` document in the `meetings` folder. You don't need to put it into a folder, **unless you need to have additional files** (e.g. images, PDF downloads, etc.).

To name the files, use the convention `YY.N-title.qmd`, where `YY` is the year, `N` is the meeting number, and `title` is a short description of the meeting.

**IMPORTANT**: set the meeting date to the date when the announcement is created. The actual (future) day when the meeting is supposed to take place and the venue shall be set in the abstract, according to the template.

Only the last meeting (more recent according to the `date` field) shows up on the site homepage. The `meetings` page, conversely, shows all the meetings.
