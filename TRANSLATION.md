# Node.js Website Translation Policy

Node.js is a global platform and so this site has many translations. The translation of the site into
languages other than English is handled by the localization working group of the language in question. If you
would like to contribute to the translation of nodejs.org, please refer to the following process:

## For Individuals wanting to contribute
* Contact your appropriate localization group, and discuss with them the best possible way to contribute. A list of the localization groups can be found here (please keep in mind that some groups have not yet taken action upon the project name changes, hence the outdated repository names):
    * [`iojs-ar`](https://github.com/nodejs/iojs-ar) Arabic Community
    * [`iojs-bg`](https://github.com/nodejs/iojs-bg) Bulgarian Community
    * [`iojs-bn`](https://github.com/nodejs/iojs-bn) Bengali Community
    * [`iojs-cn`](https://github.com/nodejs/iojs-cn) Chinese Community
    * [`iojs-cs`](https://github.com/nodejs/iojs-cs) Czech Community
    * [`iojs-da`](https://github.com/nodejs/iojs-da) Danish Community
    * [`nodejs-de`](https://github.com/nodejs/nodejs-de) German Community
    * [`iojs-el`](https://github.com/nodejs/iojs-el) Greek Community
    * [`iojs-es`](https://github.com/nodejs/iojs-es) Spanish Community
    * [`nodejs-fa`](https://github.com/nodejs/nodejs-fa) Persian Community
    * [`nodejs-fi`](https://github.com/nodejs/nodejs-fi) Finnish Community
    * [`nodejs-fr`](https://github.com/nodejs/nodejs-fr) French Community
    * [`iojs-he`](https://github.com/nodejs/iojs-he) Hebrew Community
    * [`iojs-hi`](https://github.com/nodejs/iojs-hi) Hindi Community
    * [`iojs-hu`](https://github.com/nodejs/iojs-hu) Hungarian Community
    * [`nodejs-id`](https://github.com/nodejs/nodejs-id) Indonesian Community
    * [`iojs-it`](https://github.com/nodejs/iojs-it) Italian Community
    * [`nodejs-ja`](https://github.com/nodejs/nodejs-ja) Japanese Community
    * [`nodejs-ka`](https://github.com/nodejs/nodejs-ka) Georgian Community
    * [`nodejs-ko`](https://github.com/nodejs/nodejs-ko) Korean Community
    * [`nodejs-mk`](https://github.com/nodejs/nodejs-mk) Macedonian Community
    * [`iojs-ms`](https://github.com/nodejs/iojs-ms) Malaysian Community
    * [`nodejs-nl`](https://github.com/nodejs/nodejs-nl) Dutch Community
    * [`nodejs-no`](https://github.com/nodejs/nodejs-no) Norwegian Community
    * [`iojs-pl`](https://github.com/nodejs/iojs-pl) Polish Community
    * [`iojs-pt`](https://github.com/nodejs/iojs-pt) Portuguese Community
    * [`nodejs-ro`](https://github.com/nodejs/nodejs-ro) Romanian Community
    * [`iojs-ru`](https://github.com/nodejs/iojs-ru) Russian Community
    * [`iojs-sv`](https://github.com/nodejs/iojs-sv) Swedish Community
    * [`nodejs-ta`](https://github.com/nodejs/nodejs-ta) Tamil Community
    * [`nodejs-tr`](https://github.com/nodejs/nodejs-tr) Turkish Community
    * [`iojs-tw`](https://github.com/nodejs/iojs-tw) Taiwan Community
    * [`nodejs-uk`](https://github.com/nodejs/nodejs-uk) Ukrainian Community
    * [`iojs-vi`](https://github.com/nodejs/iojs-vi) Vietnamese Community

## For Localization Groups
* Ensure that any site translations are done as pull requests into the appropriate language folder in this repo. This will ensure the build process, layout, and styling, remain consistent across the different translations of the site.
* You can find the appropriate language folder within `locale/`
* The following files need to be in your language folder:
    * `site.json` (this contains the basic settings for the website version and the button and title bar translations)
    * `index.md` (this contains the markdown translation for the home page. The paragraph order is important here, so please maintain it)
    * `styles.styl` (this imports the necessary Stylus files)
    * All files and files in subfolders that end in `.md` are content pages and should be translated.
* Prefix your PR with the localization group's name (e.g. `nodejs-no`). If you are only translating one of the above files, please mention them in your PR's subject as well, e.g.:
```
    nodejs-de: Add files - index.md, faq.md
    nodejs-ro: Add files - 15 files

    nodejs-fr: Update files - es6.md
    nodejs-ja: Update files - all files
```
* Do not make language specific changes to layout or styling in a translation PR. If they are needed, make a separate styling/layout pr and talk with one of the website WG about the change. We want to make sure, for example, a Chinese layout change doesn't cascade failure to the German page.
* To be merged, translation PR's require a Website WG +1 and a +1 from another native speaker in your language. Make sure whoever you have review the PR adds a +1 in the comments of it so we know it is translated properly.