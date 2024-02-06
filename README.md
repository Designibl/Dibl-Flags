# Dibl Flags 🚩

Open Source Feature flag implementation examples on a Supabase backend.

N.B. Can be easily adapted for any other Postgres database.

---

## Using This Repository

This repository serves as example code that can be re-used in your own projects
to set up feature flagging capabilities rather than paing out for a service.

## Features/Examples

- [ ] Basic Boolean flag
- [ ] Basic JSON flag
- [ ] Flag Schedules
- [ ] Flag User Subsets
- [ ] A/B test
- [ ] Feature Preview
- [ ] Flag Editing UI
- [ ] Flag Sign Off Process

---

## Working On This Repository

Either fork the repository or pull it locally.

### Environment Variables

Ensure you have a `.env.local` file with the required environment variables set out
in `.env.example`.

You will receive errors on running the application if environment variables are not found.

New environment variables must be also configured in `./src/env.js`.

### Running Locally

_N.B._ We are using `bun` as our javascript runtime which is different from `npm` or `yarn`. [Find out more](https://bun.sh/)

#### First time setup install

_N.B._ These commands are meant to be run from the top level of the repository.

```bash
bun install
```

Run the development server:

```bash
bun dev
```

### Committing Code

We use the conventional commits standard to indicate version bumps.

- `fix` — to indicate a bug fix (PATCH) ex. v0.0.1
- `feat` — to indicate a new feature (MINOR) ex. v0.1.0
- `chore` — for updates that do not require a version bump (.gitignore, comments, etc.)
- `docs` — for updates to the documentation
- `BREAKING CHANGE` — regardless of type, indicates a Major release (MAJOR) ex. v1.0.0

### Preparing your PR

#### Versioning

We use a library called [Standard-Version](https://github.com/conventional-changelog/standard-version)

Run the release script:

```bash
bun release
```

And push the created changes.

This automatically:

- Generates a changelog from your commit messages.
- Bumps the version numbers in `package.json`.
- Creates a new tags with the version number.

### Deploying A Release

We use Vercel for our builds and deployment.

Create a PR, then it will automatically generate a preview build and run our github actions.

On a successful PR merge to the `trunk` branch a production build will be kicked off.

---

### Main Technologies

If you are not familiar with the different technologies used in this project, please refer to the respective docs.

This was originally setup with [T3 Stack](https://create.t3.gg/).

- [Next.js](https://nextjs.org)
- [Tailwind CSS](https://tailwindcss.com)

---

- [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
- [Markdown Emoji Cheatsheet](https://gist.github.com/rxaviers/7360908)
- [Markdown CodeBlock Language List](https://github.com/github/linguist/blob/master/lib/linguist/languages.yml)
- [Mermaid Diagram Visual Editor](https://mermaid.live)
