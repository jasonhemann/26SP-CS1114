# CS1114 Course Website

Course site built with Jekyll (GitHub Pages toolchain) and based on Minimal Mistakes.

## Required Toolchain

For local development and testing, install:

1. Ruby `3.3.4` (see [`.ruby-version`](.ruby-version))
2. Bundler (Ruby gem package manager)
3. Git

## Local Setup

Install Ruby dependencies:

```bash
bundle install
```

Build the site once (CI-like check):

```bash
bundle exec jekyll build
```

Run locally with live reload:

```bash
bundle exec jekyll serve --livereload
```

Then open: `http://127.0.0.1:4000/26SP-CS1114/`

## Contributor Workflow (TAs)

### 1) Add/update course personnel

At the start of each semester, update [`_data/personnel.yaml`](_data/personnel.yaml).

Each entry should include:

- `name`
- `role` (for example `Tutor`, `Learning Assistant`, `Instructor`)
- `email`
- `office_hours`

The TA Staff table on [`people.md`](people.md) renders this file directly.

### 2) Adjust syllabus content

Primary syllabus source: [`syllabus.md`](syllabus.md)

Typical loop:

1. Edit `syllabus.md`
2. Run `bundle exec jekyll serve --livereload`
3. Review `http://127.0.0.1:4000/26SP-CS1114/syllabus/`
4. Validate with `bundle exec jekyll build`

### 3) Adjust schedule and assignment metadata

Schedule data lives in [`_data/schedule.yml`](_data/schedule.yml), and the page template is [`schedule.md`](schedule.md).

Starter files and assignment descriptions are under [`_starter_code/`](_starter_code/).

Typical loop:

1. Edit `_data/schedule.yml` and/or `_starter_code/*`
2. Run local server (`bundle exec jekyll serve --livereload`)
3. Review `http://127.0.0.1:4000/26SP-CS1114/schedule/`
4. Validate with `bundle exec jekyll build`

## Notes

- The first `jekyll build`/`jekyll serve` on a new machine needs internet access to download the remote theme.
- Inherited `.github` issue/PR filing templates from the upstream theme were intentionally removed for this course repo.
