# Contributing to Slides

Thank you for contributing to Slides!

Please take a moment to review this document in order to make the contribution process easy and effective for everyone involved.

Following these guidelines helps to communicate that you respect the time of the developers managing and developing this open-source project. In return, and in accordance with this project's [code of conduct](.github/CODE_OF_CONDUCT.md), other contributors will reciprocate that respect in addressing your issue or assessing patches and features.

<a id="contents"></a>

## **Contents**

- [Tech stack](#tech-stack-)
- [Learning the tech stack](#learning-the-tech-)
- [Development environment](#dev-env-)
- [Issues](#issues-)
- [Bug reports](#bug-reports-)
- [Feature requests](#feature-requests-)
- [Pull requests](#pull-requests-)

<a id="tech-stack-"></a>

## Tech Stack [`⇧`](#contents)

The following are the current technologies used in Slides:

### Frontend

- [Slidev](https://sli.dev/) • [Vue.js](https://vuejs.org) • [UnoCSS](https://unocss.dev/)

> [!NOTE]
> Those new to any frameworks or technologies who want to work on their skills are more than welcome to contribute!

<a id="learning-the-tech-"></a>

## Learning the tech stack [`⇧`](#contents)

Slides is very open to contributions from people in the early stages of their coding journey! The following is a select list of documentation pages to help you understand the technologies we use.

<details><summary>Docs for those new to programming</summary>
<p>

- [Mozilla Developer Network Learning Area](https://developer.mozilla.org/en-US/docs/Learn)
  - Doing MDN sections for HTML, CSS and JavaScript is the best ways to get into web development!
- [Open Source Guides](https://opensource.guide/)
  - Guides from GitHub about open-source software including how to start and much more!

</p>
</details>

<details><summary>Slides tech docs</summary>
<p>

- [Vue.js 3 docs](https://vuejs.org/guide/introduction.html)
- [Vue docs on MDN](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Client-side_JavaScript_frameworks/Vue_getting_started)
- [UnoCSS docs](https://unocss.dev/interactive/)

</p>
</details>

<a id="dev-env-"></a>

## Development environment [`⇧`](#contents)

1. First and foremost, please see the suggested IDE setup in the dropdown below to make sure that your editor is ready for development.

> [!IMPORTANT]
>
> <details><summary>Suggested IDE setup</summary>
>
> <p>
>
> VS Code
>
> Install the following extensions:
>
> - [esbenp.prettier-vscode](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
> - [streetsidesoftware.code-spell-checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker)
> - [Vue.volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar)
>
> </p>
> </details>

2. [Fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) the [Slides repo](https://github.com/scribe-org/slides), clone your fork, and configure the remotes:

> [!NOTE]
>
> <details><summary>Consider using SSH</summary>
>
> <p>
>
> Alternatively to using HTTPS as in the instructions below, consider SSH to interact with GitHub from the terminal. SSH allows you to connect without a user-pass authentication flow.
>
> To run git commands with SSH, remember then to substitute the HTTPS URL, `https://github.com/...`, with the SSH one, `git@github.com:...`.
>
> - e.g. Cloning now becomes `git clone git@github.com:<your-username>/slides.git`
>
> GitHub also has their documentation on how to [Generate a new SSH key](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) 🔑
>
> </p>
> </details>

```bash
# Clone your fork of the repo into the current directory.
git clone https://github.com/<your-username>/slides.git
# Navigate to the newly cloned directory.
cd slides
# Assign the original repo to a remote called "upstream".
git remote add upstream https://github.com/scribe-org/slides.git
```

- Now, if you run `git remote -v` you should see two remote repositories named:
  - `origin` (forked repository)
  - `upstream` (Slides repository)

3. Install the dependencies for all presentations including making [Prettier](https://prettier.io/) format `slides.md` files via the top level [package.json](package.json) and [.prettierrc](.prettierrc) files:

```bash
# Based on your package manager:
yarn install
npm install
pnpm install
```

4. Build and open your slides of choice by navigating to its directory and executing the `run dev` command for your package manager:

```bash
cd SLIDES_OF_CHOICE

# Based on your package manager:
yarn run dev
npm run dev
pnpm run dev
```

5. Once finished you can visit <http://localhost:3030> to view the slides. Follow the prompts in your terminal to close them or do other actions.

<a id="issues-"></a>

## Issues [`⇧`](#contents)

The [issue tracker for Slides](https://github.com/scribe-org/slides/issues) is the preferred channel for [bug reports](#bug-reports), [features requests](#feature-requests) and [submitting pull requests](#pull-requests).

Be sure to check the [`-priority-`](https://github.com/scribe-org/slides/labels/-priority-) labels in the [issues](https://github.com/scribe-org/slides/issues) for those that are most important, as well as those marked [`good first issue`](https://github.com/scribe-org/slides/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) that are tailored for first time contributors.

<a name="bug-reports"></a>

## Bug reports [`⇧`](#contents)

A bug is a _demonstrable problem_ that is caused by the code in the repository. Good bug reports are extremely helpful — thank you!

Guidelines for bug reports:

1. **Use the GitHub issue search** to check if the issue has already been reported.

2. **Check if the issue has been fixed** by trying to reproduce it using the latest `main` or development branch in the repository.

3. **Isolate the problem** to make sure that the code in the repository is _definitely_ responsible for the issue.

**Great Bug Reports** tend to have:

- A quick summary
- Steps to reproduce
- What you expected would happen
- What actually happens
- Notes (why this might be happening, things tried that didn't work, etc)

To make the above steps easier, the Slides team asks that contributors report bugs using the [bug report template](https://github.com/scribe-org/slides/issues/new?assignees=&labels=bug&template=bug_report.yml), with these issues further being marked with the [`bug`](https://github.com/scribe-org/slides/issues?q=is%3Aopen+is%3Aissue+label%3Abug) label.

Again, thank you for your time in reporting issues!

<a name="feature-requests-"></a>

## Feature requests [`⇧`](#contents)

Feature requests are more than welcome! Please take a moment to find out whether your idea fits with the scope and aims of the project. When making a suggestion, provide as much detail and context as possible, and further make clear the degree to which you would like to contribute in its development. Feature requests are marked with the [`feature`](https://github.com/scribe-org/slides/issues?q=is%3Aopen+is%3Aissue+label%3Afeature) label in the [issues](https://github.com/scribe-org/slides/issues).

<a name="pull-requests-"></a>

## Pull requests [`⇧`](#contents)

Good pull requests — patches, improvements and new features — are the foundation of our community making Slides. They should remain focused in scope and avoid containing unrelated commits. Note that all contributions to this project will be made under [the specified license](LICENSE.txt) and should follow the coding indentation and style standards (contact us if unsure).

**Please ask first** before embarking on any significant pull request (implementing features, refactoring code, etc), otherwise you risk spending a lot of time working on something that the developers might not want to merge into the project. With that being said, major additions are very appreciated!

When making a contribution, adhering to the [GitHub flow](https://docs.github.com/en/get-started/quickstart/github-flow) process is the best way to get your work merged:

1. If you cloned a while ago, get the latest changes from upstream:

   ```bash
   git checkout <dev-branch>
   git pull upstream <dev-branch>
   ```

2. Create a new topic branch (off the main project development branch) to contain your feature, change, or fix:

   ```bash
   git checkout -b <topic-branch-name>
   ```

3. Install [pre-commit](https://pre-commit.com/) to ensure that each of your commits is properly checked against our linter and formatters:

   ```bash
   # In the project root:
   pre-commit install
   ```

> [!NOTE]
> pre-commit is Python package that can be installed via pip or any other Python package manager. You can also find it in our [requirements.txt](backend/requirements.txt) file.
>
> ```bash
> pip install pre-commit
> ```

> [!NOTE]
> If you are having issues with pre-commit and want to send along your changes regardless, you can ignore the pre-commit hooks via the following:
>
> ```bash
> git commit --no-verify -m "COMMIT_MESSAGE"
> ```

4. Commit your changes in logical chunks, and please try to adhere to [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).

> [!NOTE]
> The following are tools and methods to help you write good commit messages ✨
>
> - [commitlint](https://commitlint.io/) helps write [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)
> - Git's [interactive rebase](https://docs.github.com/en/github/getting-started-with-github/about-git-rebase) cleans up commits

5. Locally merge (or rebase) the upstream development branch into your topic branch:

   ```bash
   git pull --rebase upstream <dev-branch>
   ```

6. Push your topic branch up to your fork:

   ```bash
   git push origin <topic-branch-name>
   ```

7. [Open a Pull Request](https://help.github.com/articles/using-pull-requests/) with a clear title and description.

Thank you in advance for your contributions!
