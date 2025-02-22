> ## 🚨 Important Notice
>
> This repository is a clone of the
> [React Suspense legacy-module](https://github.com/kentcdodds/react-suspense)
> by Kent C. Dodds. It has been published solely to document my GitHub activity
> and for personal educational purposes.
>
> **Note:** This is not an official fork or a maintained derivative of the
> original project.

<div>
  <h1 align="center"><a href="https://www.epicreact.dev/modules/react-suspense-v1/react-suspense-welcome">🔀 React Suspense 🚀 EpicReact.Dev</a></h1>
  <strong>
    Simplify your Async UI and improve your User Experience
  </strong>
  <p>
    Learn how Suspense works under the hood, preparing you for the future of asynchronous state management.
  </p>

  <a href="https://epicreact.dev">
    <img
      alt="Learn React from Start to Finish"
      src="https://kentcdodds.com/images/epicreact-promo/er-1.gif"
    />
  </a>
</div>

<hr />

<!-- prettier-ignore-start -->
[![Build Status][build-badge]][build]
[![All Contributors][all-contributors-badge]](#contributors)
[![GPL 3.0 License][license-badge]][license]
[![Code of Conduct][coc-badge]][coc]
[![Gitpod ready-to-code][gitpod-badge]](https://gitpod.io/#https://github.com/kentcdodds/react-suspense)
<!-- prettier-ignore-end -->

## ⚠️ Warning ⚠️

This workshop material deals with **EXPERIMENTAL** features in React. Please do
not copy/paste any of the code you find here into a production application and
expect it to work. The features have been released in the latest version of
React 18 and there are some slight changes. However the concepts and most APIs
taught in this workshop are still applicable (any changes are noted in the
material).

## NOTICE:

This workshop deals a lot with error boundaries and it's important to note that
create-react-app has a special and helpful "Error Overlay" component that will
sometimes be displayed when an error occurs (whether your app implements error
boundaries or not). For you to see the error handling within the app, you'll
need to close that overlay by clicking the "x" in the upper-right.

## Prerequisites

- Install the React DevTools
  ([Chrome](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en)
  (recommended),
  [Firefox](https://addons.mozilla.org/en-US/firefox/addon/react-devtools/))
- Watch Dan Abramov's talk
  [Beyond React 16 | JSConf Iceland 2018](https://www.youtube.com/watch?v=nLF0n9SACd4)
  (33 minutes)
- Experience with React and all hooks

## Quick start

It's recommended you run everything in the same environment you work in every
day, but if you don't want to set up the repository locally, you can get started
in one click with [Gitpod](https://gitpod.io),
[CodeSandbox](https://codesandbox.io/s/github/kentcdodds/react-suspense), or by
following the [video demo](https://www.youtube.com/watch?v=gCoVJm3hGk4)
instructions for [GitHub Codespaces](https://github.com/features/codespaces).

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/kentcdodds/react-suspense)

For a local development environment, follow the instructions below

## System Requirements

- [git][git] v2.13 or greater
- [NodeJS][node] `>=16`
- [npm][npm] v8.16.0 or greater

All of these must be available in your `PATH`. To verify things are set up
properly, you can run this:

```shell
git --version
node --version
npm --version
```

If you have trouble with any of these, learn more about the PATH environment
variable and how to fix it here for [windows][win-path] or
[mac/linux][mac-path].

## Setup

> If you want to commit and push your work as you go, you'll want to
> [fork](https://docs.github.com/en/free-pro-team@latest/github/getting-started-with-github/fork-a-repo)
> first and then clone your fork rather than this repo directly.

After you've made sure to have the correct things (and versions) installed, you
should be able to just run a few commands to get set up:

```shell
git clone https://github.com/kentcdodds/react-suspense.git
cd react-suspense
node setup
```

This may take a few minutes. **It will ask you for your email.** This is
optional and just automatically adds your email to the links in the project to
make filling out some forms easier.

If you get any errors, please read through them and see if you can find out what
the problem is. If you can't work it out on your own then please [file an
issue][issue] and provide _all_ the output from the commands you ran (even if
it's a lot).

If you can't get the setup script to work, then just make sure you have the
right versions of the requirements listed above, and run the following commands:

```shell
npm install
npm run validate
```

If you are still unable to fix issues and you know how to use Docker 🐳 you can
setup the project with the following command:

```shell
docker-compose up
```

## Running the app

To get the app up and running (and really see if it worked), run:

```shell
npm start
```

This should start up your browser. If you're familiar, this is a standard
[react-scripts](https://create-react-app.dev/) application.

You can also open
[the deployment of the app on Netlify](https://react-suspense.netlify.app/).

## Running the tests

```shell
npm test
```

This will start [Jest](https://jestjs.io/) in watch mode. Read the output and
play around with it. The tests are there to help you reach the final version,
however _sometimes_ you can accomplish the task and the tests still fail if you
implement things differently than I do in my solution, so don't look to them as
a complete authority.

### Exercises

- `src/exercise/00.md`: Background, Exercise Instructions, Extra Credit
- `src/exercise/00.js`: Exercise with Emoji helpers
- `src/__tests__/00.js`: Tests
- `src/final/00.js`: Final version
- `src/final/00.extra-0.js`: Final version of extra credit

The purpose of the exercise is **not** for you to work through all the material.
It's intended to get your brain thinking about the right questions to ask me as
_I_ walk through the material.

### Helpful Emoji 🐨 💰 💯 📝 🦉 📜 💣 💪 🏁 👨‍💼 🚨

Each exercise has comments in it to help you get through the exercise. These fun
emoji characters are here to help you.

- **Kody the Koala** 🐨 will tell you when there's something specific you should
  do
- **Marty the Money Bag** 💰 will give you specific tips (and sometimes code)
  along the way
- **Hannah the Hundred** 💯 will give you extra challenges you can do if you
  finish the exercises early.
- **Nancy the Notepad** 📝 will encourage you to take notes on what you're
  learning
- **Olivia the Owl** 🦉 will give you useful tidbits/best practice notes and a
  link for elaboration and feedback.
- **Dominic the Document** 📜 will give you links to useful documentation
- **Berry the Bomb** 💣 will be hanging around anywhere you need to blow stuff
  up (delete code)
- **Matthew the Muscle** 💪 will indicate that you're working with an exercise
- **Chuck the Checkered Flag** 🏁 will indicate that you're working with a final
- **Peter the Product Manager** 👨‍💼 helps us know what our users want
- **Alfred the Alert** 🚨 will occasionally show up in the test failures with
  potential explanations for why the tests are failing.

## Contributors

Thanks goes to these wonderful people
([emoji key](https://github.com/kentcdodds/all-contributors#emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://kentcdodds.com"><img src="https://avatars.githubusercontent.com/u/1500684?v=3?s=100" width="100px;" alt="Kent C. Dodds"/><br /><sub><b>Kent C. Dodds</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=kentcdodds" title="Code">💻</a> <a href="https://github.com/kentcdodds/react-suspense/commits?author=kentcdodds" title="Documentation">📖</a> <a href="#infra-kentcdodds" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/kentcdodds/react-suspense/commits?author=kentcdodds" title="Tests">⚠️</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Hypnosphi"><img src="https://avatars3.githubusercontent.com/u/6651625?v=4?s=100" width="100px;" alt="Filipp Riabchun"/><br /><sub><b>Filipp Riabchun</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=Hypnosphi" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/lauchness"><img src="https://avatars0.githubusercontent.com/u/51837850?v=4?s=100" width="100px;" alt="lauchness"/><br /><sub><b>lauchness</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=lauchness" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/pritamsangani/"><img src="https://avatars3.githubusercontent.com/u/22857896?v=4?s=100" width="100px;" alt="Pritam Sangani"/><br /><sub><b>Pritam Sangani</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=PritamSangani" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/emzoumpo"><img src="https://avatars2.githubusercontent.com/u/2103443?v=4?s=100" width="100px;" alt="Emmanouil Zoumpoulakis"/><br /><sub><b>Emmanouil Zoumpoulakis</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=emzoumpo" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="http://peter.hozak.info/"><img src="https://avatars0.githubusercontent.com/u/1087670?v=4?s=100" width="100px;" alt="Peter Hozák"/><br /><sub><b>Peter Hozák</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=Aprillion" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="http://twitter.com/jcarty"><img src="https://avatars1.githubusercontent.com/u/952914?v=4?s=100" width="100px;" alt="Jerome Carty"/><br /><sub><b>Jerome Carty</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=jcarty" title="Code">💻</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="http://anthonyng.me"><img src="https://avatars1.githubusercontent.com/u/14035529?v=4?s=100" width="100px;" alt="Anthony Ng"/><br /><sub><b>Anthony Ng</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=newyork-anthonyng" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://vk.com/vasilii_kovalev"><img src="https://avatars0.githubusercontent.com/u/10310491?v=4?s=100" width="100px;" alt="Vasilii Kovalev"/><br /><sub><b>Vasilii Kovalev</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/issues?q=author%3Avasilii-kovalev" title="Bug reports">🐛</a> <a href="https://github.com/kentcdodds/react-suspense/commits?author=vasilii-kovalev" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://michaeldeboey.be"><img src="https://avatars3.githubusercontent.com/u/6643991?v=4?s=100" width="100px;" alt="Michaël De Boey"/><br /><sub><b>Michaël De Boey</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=MichaelDeBoey" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dsod"><img src="https://avatars0.githubusercontent.com/u/19597385?v=4?s=100" width="100px;" alt="Daniel Söderling"/><br /><sub><b>Daniel Söderling</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=dsod" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="http://bobbywarner.com"><img src="https://avatars0.githubusercontent.com/u/554961?v=4?s=100" width="100px;" alt="Bobby Warner"/><br /><sub><b>Bobby Warner</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=bobbywarner" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="http://angular-tips.com"><img src="https://avatars2.githubusercontent.com/u/1087957?v=4?s=100" width="100px;" alt="Jesús Rodríguez"/><br /><sub><b>Jesús Rodríguez</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=Foxandxss" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/cesarcf"><img src="https://avatars0.githubusercontent.com/u/5168360?v=4?s=100" width="100px;" alt="Cesar Carbajo"/><br /><sub><b>Cesar Carbajo</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=cesarcf" title="Code">💻</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/waxidiotic"><img src="https://avatars1.githubusercontent.com/u/8037469?v=4?s=100" width="100px;" alt="Alex Bussey"/><br /><sub><b>Alex Bussey</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=waxidiotic" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/intrueder"><img src="https://avatars2.githubusercontent.com/u/182339?v=4?s=100" width="100px;" alt="Tymur Mudzhyri"/><br /><sub><b>Tymur Mudzhyri</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/issues?q=author%3Aintrueder" title="Bug reports">🐛</a> <a href="https://github.com/kentcdodds/react-suspense/commits?author=intrueder" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/billfienberg"><img src="https://avatars3.githubusercontent.com/u/6130520?v=4?s=100" width="100px;" alt="Bill Fienberg"/><br /><sub><b>Bill Fienberg</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=billfienberg" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="http://devlogger.wordpress.com"><img src="https://avatars2.githubusercontent.com/u/15407?v=4?s=100" width="100px;" alt="Martin Carel"/><br /><sub><b>Martin Carel</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=cawel" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://gkueny.fr"><img src="https://avatars.githubusercontent.com/u/10655690?v=4?s=100" width="100px;" alt="Gaëtan Kueny"/><br /><sub><b>Gaëtan Kueny</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/issues?q=author%3Agkueny" title="Bug reports">🐛</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/nawok"><img src="https://avatars.githubusercontent.com/u/159773?v=4?s=100" width="100px;" alt="Pavel Fomchenkov"/><br /><sub><b>Pavel Fomchenkov</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/issues?q=author%3Anawok" title="Bug reports">🐛</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://plai.team"><img src="https://avatars.githubusercontent.com/u/6297446?v=4?s=100" width="100px;" alt="Andriy Bas"/><br /><sub><b>Andriy Bas</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=AndriyBas" title="Code">💻</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="http://pavlos.dev"><img src="https://avatars.githubusercontent.com/u/100233?v=4?s=100" width="100px;" alt="Pavlos Vinieratos"/><br /><sub><b>Pavlos Vinieratos</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=pvinis" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/marioleed"><img src="https://avatars.githubusercontent.com/u/1763448?v=4?s=100" width="100px;" alt="Mario Sannum"/><br /><sub><b>Mario Sannum</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=marioleed" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="http://www.lucianoayres.com.br"><img src="https://avatars.githubusercontent.com/u/20209393?v=4?s=100" width="100px;" alt="Luciano Ayres"/><br /><sub><b>Luciano Ayres</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=lucianoayres" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="http://jasik.xyz"><img src="https://avatars.githubusercontent.com/u/10626596?v=4?s=100" width="100px;" alt="Caleb Jasik"/><br /><sub><b>Caleb Jasik</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=jasikpark" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/PhilippVujic"><img src="https://avatars.githubusercontent.com/u/28774924?v=4?s=100" width="100px;" alt="Philipp Vujic"/><br /><sub><b>Philipp Vujic</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=PhilippVujic" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/OptimalEmre"><img src="https://avatars.githubusercontent.com/u/73573610?v=4?s=100" width="100px;" alt="Emre"/><br /><sub><b>Emre</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=OptimalEmre" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://creador.dev"><img src="https://avatars.githubusercontent.com/u/40248406?v=4?s=100" width="100px;" alt="Pawan Kumar"/><br /><sub><b>Pawan Kumar</b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=creador-dev" title="Documentation">📖</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Creeland"><img src="https://avatars.githubusercontent.com/u/518406?v=4?s=100" width="100px;" alt="Creeland A. Provinsal "/><br /><sub><b>Creeland A. Provinsal </b></sub></a><br /><a href="https://github.com/kentcdodds/react-suspense/commits?author=Creeland" title="Documentation">📖</a></td>
    </tr>
  </tbody>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the
[all-contributors](https://github.com/kentcdodds/all-contributors)
specification. Contributions of any kind welcome!

## Workshop Feedback

Each exercise has an Elaboration and Feedback link. Please fill that out after
the exercise and instruction.

At the end of the workshop, please go to this URL to give overall feedback.
Thank you! https://kcd.im/rs-ws-feedback

<!-- prettier-ignore-start -->
[npm]: https://www.npmjs.com/
[node]: https://nodejs.org
[git]: https://git-scm.com/
[build-badge]: https://img.shields.io/github/actions/workflow/status/kentcdodds/react-suspense/validate.yml?branch=main&logo=github&style=flat-square
[build]: https://github.com/kentcdodds/react-suspense/actions?query=workflow%3Avalidate
[license-badge]: https://img.shields.io/badge/license-GPL%203.0%20License-blue.svg?style=flat-square
[license]: https://github.com/kentcdodds/react-suspense/blob/main/LICENSE
[coc-badge]: https://img.shields.io/badge/code%20of-conduct-ff69b4.svg?style=flat-square
[gitpod-badge]: https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod
[coc]: https://github.com/kentcdodds/react-suspense/blob/main/CODE_OF_CONDUCT.md
[emojis]: https://github.com/kentcdodds/all-contributors#emoji-key
[all-contributors]: https://github.com/kentcdodds/all-contributors
[all-contributors-badge]: https://img.shields.io/github/all-contributors/kentcdodds/react-suspense?color=orange&style=flat-square
[win-path]: https://www.howtogeek.com/118594/how-to-edit-your-system-path-for-easy-command-line-access/
[mac-path]: http://stackoverflow.com/a/24322978/971592
[issue]: https://github.com/kentcdodds/react-suspense/issues/new
<!-- prettier-ignore-end -->
