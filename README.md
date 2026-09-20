# Course Specification Builder

A single-page form that produces a `course-specification.json` file describing
a semester course: its units and topics, learning outcomes, assignments,
grading weights, in-class methods, and delivery.

Published at **https://rhhm.github.io/course-form/** — replace with the real
URL once GitHub Pages is switched on.

Operated by **RHHM LLC**.

## What it is

One HTML file. No build step, no dependencies, no server, no analytics, no
tracking. Everything happens in the browser:

- Nothing is transmitted anywhere. The page makes no network requests except
  for its web fonts.
- Work in progress is kept in the browser's own local storage so a closed tab
  does not lose it. That data never leaves the machine it was typed on.
- The form produces a file. The person downloads it and emails it on. That is
  the whole transport mechanism, and it is deliberate — a form that posted
  somewhere would need a server, an endpoint to secure, and a privacy policy.

## Using it

Fill in the seven steps, then **Download JSON** and email the file to the
address shown on the last step.

As you type, the form checks its own input: weights that do not total 100%,
outcomes phrased so that nothing observable could be assessed, sessions that
are not real session numbers. Errors block the download and link straight to
the field that needs fixing. Suggestions — on learning outcomes in particular
— never block anything.

## Running it locally

```bash
open index.html
```

That is all. It works from a `file://` URL exactly as it does when hosted.

## Publishing

GitHub Pages, serving from the repository root. `index.html` is the whole site.

## License

MIT. Copyright (c) 2026 RHHM LLC.
