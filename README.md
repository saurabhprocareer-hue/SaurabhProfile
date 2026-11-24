# saurabhProfile

Personal profile website for **Saurabh Singhal** — Engineering Manager · Cloud Transformation · AI Orchestration.

A static site (plain HTML/CSS/JS, no build step) with sections for achievements, latest learning & certificates, white papers, design architecture, experience and contact.

## Structure

```
index.html                       Profile site
whitepapers/us-healthcare.html   White paper: Medical Tourism to India
README.md
```

## Updating content

All profile content lives in the **DATA** block near the bottom of `index.html`. Add an object to the relevant list and the page renders it automatically:

| List | Section |
|---|---|
| `ACHIEVEMENTS` | Achievements (filterable by `category`) |
| `LEARNING` | Latest learning timeline |
| `CERTIFICATES` | Certificates & education (optional `link`) |
| `WHITEPAPERS` | White papers (`status`, `date`, `link`) |
| `ARCHITECTURE` | Design architecture (`layers` are drawn as a diagram) |
| `EXPERIENCE`, `TOOLKIT` | Experience and technology toolkit |

To add a new white paper, create `whitepapers/<name>.html` (copy `us-healthcare.html` as a template) and add an entry to `WHITEPAPERS` with `link:"whitepapers/<name>.html"`.

## Publishing with GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`.
3. The site will be live at `https://<username>.github.io/saurabhProfile/`.
