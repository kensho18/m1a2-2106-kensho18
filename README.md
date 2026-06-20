# Module 1 – Activity 1 – Create a Basic Webpage

Your first activity. Build a complete, valid HTML5 webpage from scratch and
fill in your details.

## What to do

### 1. Fill in your details

Open `student.json` and fill in every field:

```json
{
  "classCode": "1234",
  "fullName": "Juan Dela Cruz",
  "studentNumber": "2026-12345",
  "studentEmail": "juan.delacruz@hau.edu.ph",
  "personalEmail": "juan@example.com",
  "githubAccount": "juandelacruz"
}
```

Use the **class code** your instructor gave you (it also appears in your repo
name, e.g. `m1a1-1234-yourname`). This file **is** committed to your repo, so
the tests can read it. Don't put passwords or secrets here.

> **Keep `student.json` identical across all your activities.** The autograder
> cross-checks these fields between your repos, and a mismatch (e.g. a different
> `classCode` in one activity) is flagged. The `classCode` must also match the
> one in your repo name.

### 2. Build the webpage

> **Work in the [`src/`](src/) folder.** That is the only folder you edit. Your
> webpage files (now and in later activities) live there. Everything else in
> this repo (`test/`, `package.json`, `.github/`) is course plumbing — leave it
> alone.

Open [`src/index.html`](src/index.html). It contains only a comment describing
what to build. Replace it with a complete HTML5 page that includes:

1. The **HTML5 document type declaration** on the first line.
2. The **root element** that wraps the whole page, with its **language**
   attribute set to English.
3. A **head** section containing the page **title** (shown on the browser tab)
   and the **character-encoding** declaration (UTF-8).
4. A **body** section with a **heading or paragraph** that welcomes the
   visitor (for example, `Welcome to My First Webpage`).

The comment in `src/index.html` names each tag to research in Chapter 1. Look
the tags up and write them yourself — that is the point of the activity.

### 3. View it in a browser

Double-click `src/index.html` (or right-click → *Open with* your browser). You
should see your welcome message and your title on the browser tab.

## Set up your repo

Before you write any code, create **your own copy** of this activity from the
template. Do not work in the template itself.

1. **Create from the template.** Open the template repo and click
   **Use this template → Create a new repository**.
2. **Set the owner to the course org.** Under *Owner*, choose the
   **`HAU-6INTROWEB` course org**, **not** your personal account.
3. **Name it by the convention** `m<module>a<activity>-<classcode>-<yourname>`.
   For this activity that's **`m1a1-<classcode>-yourname`** (e.g.
   `m1a1-1234-juandelacruz`). The `<classcode>` must match the one you put in
   `student.json`.
4. **Make it Private.** Set *Visibility* to **Private** so classmates can't see
   your work.

Then clone **your** new repo and work there:

```bash
git clone https://github.com/HAU-6INTROWEB/m1a1-<classcode>-yourname.git
cd m1a1-<classcode>-yourname
```

## Running the tests

Install dependencies once:

```bash
npm install
```

Then run the tests:

```bash
npm test
```

This activity is graded by **6 tests** (1 point each). They check:

- ✅ `src/index.html` declares the HTML5 doctype
- ✅ the `<html>` element has a `lang` attribute
- ✅ the page has a non-empty `<title>`
- ✅ the page declares its character encoding (`<meta charset="utf-8">`)
- ✅ the body shows a welcome heading or paragraph with text
- ✅ `student.json` is completely filled in

Each part is graded independently, so you earn partial credit for the parts
you finish.

## Confirm your submission

Your repo **is** your submission, so there is nothing to upload anywhere.
**Pushing your work is how you submit it.** When your tests pass locally,
**commit and push**:

```bash
git add -A
git commit -m "Activity 1 complete"
git push
```

Pushing triggers the **Autograde** workflow on GitHub. Confirm your submission
landed:

1. Open your repo on GitHub and click the **Actions** tab.
2. Open the latest **Autograde** run and confirm the green ✅ check
   and the "6 / 6 tests passed" summary.
