# CS1114 Course Website

Course site built with Jekyll (GitHub Pages toolchain) and based on Minimal Mistakes.

## Required Toolchain

For local development and testing, install:

1. Ruby `3.3.4` (see [`.ruby-version`](.ruby-version))
2. Bundler
3. Git

## Local Setup

Install Ruby dependencies:

```bash
bundle install
```

Run locally with live reload:

```bash
bundle exec jekyll serve --livereload
```

Then open: `http://127.0.0.1:4000/26SP-CS1114/`

## Contributor Workflow

### 1) Update course personnel

TA/tutoring data lives in [`_data/personnel.yaml`](_data/personnel.yaml), and the People page is rendered from [`people.md`](people.md).

Each entry should include:

- `name`
- `role`
- `email`
- `office_hours`

### 2) Update syllabus content

Primary syllabus source: [`syllabus.md`](syllabus.md)

Typical loop:

1. Edit `syllabus.md`
2. Run `bundle exec jekyll serve --livereload`
3. Review `http://127.0.0.1:4000/26SP-CS1114/syllabus/`

### 3) Update schedule and assignment materials

Schedule data lives in [`_data/schedule.yml`](_data/schedule.yml), and the page template is [`schedule.md`](schedule.md).

Starter files and assignment descriptions live under [`_starter_code/`](_starter_code/).

Typical loop:

1. Edit `_data/schedule.yml` and/or `_starter_code/*`
2. Run local server (`bundle exec jekyll serve --livereload`)
3. Review `http://127.0.0.1:4000/26SP-CS1114/schedule/`

## Notes

- The local Ruby/Jekyll toolchain is pinned in [`Gemfile`](Gemfile) and [`.ruby-version`](.ruby-version).
- The first `jekyll serve` on a new machine needs internet access to download the remote theme.
- Inherited `.github` issue/PR filing templates from the upstream theme were intentionally removed for this course repo.
