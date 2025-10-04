# 🥋 Contributing to KanaDojo

Hey there! Thanks for checking out **KanaDojo** — we're genuinely glad you're here. Whether you're fixing a typo, adding new kanji, or building a brand-new feature, your time and effort matter a lot. This project exists to make learning Japanese beautiful and fun, and we’d love for you to be part of it.

---

## 💡 What You Can Contribute

There’s more than one way to help out here. Some folks code, some write, some test, and some just ask the right questions. All are welcome.

**You can:**

* 🐛 Report bugs (spelling mistakes count too!)
* 💬 Suggest new features or UI tweaks
* 🧠 Improve documentation (like this file!)
* 🎨 Add new themes or Japanese fonts
* ✏️ Expand vocabulary and kanji datasets
* 🧩 Help with accessibility or localization
* 🧰 Refactor small pieces of code for clarity

If you’re new to open source, this is a great place to start. We’ve tagged some issues as `good first issue` to help you find friendly entry points.

---

## ⚙️ Getting Set Up

Before you jump in, make sure your environment is ready:

### Prerequisites

* **Node.js 18+**
* **npm 10+** (comes with Node)

### Setup Steps

```bash
# 1. Fork the repo
https://github.com/lingdojo/kanadojo/fork

# 2. Clone your fork
 git clone https://github.com/<your-username>/kanadojo.git
 cd kanadojo

# 3. Add the original repo as upstream (to stay in sync)
 git remote add upstream https://github.com/lingdojo/kanadojo.git

# 4. Install dependencies
 npm install

# 5. Start the dev server
 npm run dev
```

Now head to [http://localhost:3000](http://localhost:3000) and you should see KanaDojo running. You can explore the three main dojos — **Kana**, **Kanji**, and **Vocabulary** — and their game modes.

If you run into issues, try clearing the cache with:

```bash
rm -rf .next node_modules && npm install
```

That usually does the trick.

---

## 🧭 How the Project Is Structured

You’ll notice a clean layout when you open the codebase:

```
kanadojo/
├── app/                 # Next.js App Router pages
├── components/          # Reusable UI & Dojo components
├── store/               # Zustand state management
├── static/              # Kana, Kanji, and Vocabulary data
├── lib/                 # Custom hooks and utilities
├── public/              # Assets (sounds, wallpapers)
└── tailwind.config.js   # Styling setup
```

If you're here to make code changes, focus on `components/`, `store/`, or `lib/`.
If you're here for content (themes, fonts, vocab, kanji), go straight to `static/`.

---

## 🧑‍💻 Making Changes

Here’s how to keep things tidy:

1. **Create a new branch** for your change:

   ```bash
   git checkout -b feat/dark-mode-improvements
   ```

2. **Code style:**

   * We use **TypeScript** for type safety.
   * Keep components small and readable.
   * Follow Tailwind conventions and use the helper `cn()` from `lib/utils.ts`.

3. **Commit messages:**
   Use [Conventional Commits](https://www.conventionalcommits.org/) — it keeps the history neat.

   ```bash
   feat(theme): add random theme shuffle
   fix(vocab): correct typo in N5 wordlist
   docs(readme): update setup instructions
   ```

4. **Run linting before pushing:**

   ```bash
   npm run lint
   ```

5. **Test your feature manually.** Make sure all four game modes still behave correctly: Pick, Reverse-Pick, Input, Reverse-Input.

If your change affects visuals (themes, fonts, UI), take a quick screenshot or GIF for your PR. Reviewers will love you for it.

---

## 🚀 Submitting a Pull Request

When your change is ready:

1. Push your branch to your fork:

   ```bash
   git push origin feat/dark-mode-improvements
   ```

2. Open a pull request against the **`main`** branch of `lingdojo/kanadojo`.

3. In your PR description:

   * Explain what problem you solved and *why* it matters.
   * Include screenshots for visual changes.
   * Add reproduction steps if it’s a bug fix.
   * Mention related issue numbers (e.g., “Fixes #123”).

We try to review PRs within a few days, but remember: this is a volunteer-driven project. If you don’t hear back quickly, a polite ping is totally fine.

If your PR isn’t accepted right away — don’t sweat it. We’ll help you refine it.

---

## 🧩 Reporting Issues

If you find something broken or confusing, open an issue!

Please include:

* What you were trying to do
* What you expected to happen
* What actually happened (screenshots help!)
* Your browser + OS info

Before opening a new issue, check if it already exists — we might already be on it.

For feature requests, be descriptive. Tell us *why* the feature helps learners. For example:

> “Add keyboard hotkeys for fast input during Pick mode.”

That kind of detail makes it easier to prioritize.

---

## 🧠 Code of Conduct

KanaDojo follows the spirit of the [Contributor Covenant](https://www.contributor-covenant.org/). In short: be kind, be respectful, and make space for everyone to learn.

If you ever feel uncomfortable or see behavior that crosses the line, reach out privately to the maintainers through GitHub.

---

## 💬 Need Help?

If you’re stuck or just want to talk about an idea:

* Open a **GitHub Discussion** or issue.
* Drop a comment on a related PR.

We’re friendly folks — promise. 🙂

Typical response time is within a few days. We’re doing this for the love of Japanese and clean code.

---

## 🌸 A Few Final Tips

* Small PRs are easier to review than massive ones. Break things up when you can.
* Don’t worry about perfection. We’d rather have your ideas early than never.
* If something’s unclear, *ask*. That’s how we improve docs like this one.
* Be mindful that this repo is deployed on **Vercel**, so major changes may affect build times.

---

## ❤️ Thank You

Seriously — thanks for taking the time to read this. Every contribution, big or small, keeps KanaDojo growing.

がんばって! (Ganbatte — do your best!)
