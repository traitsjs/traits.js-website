# traits.js website

Sources for the [traits.js website](https://traitsjs.github.io/traits.js-website/).

## Running locally

To run locally: [`jekyll serve`](https://jekyllrb.com/docs/quickstart/)

To update the `traits.js` repo:
1. After `git clone`/`git pull`, do `git submodule update`
2. Then `cd traits.js`
3. and `git checkout master`.
4. Now you can do `git pull`.
5. To save your update, do `cd ..` and `git commit traits.js -m "updated traits.js"`

If you do work in the `traits.js` submodule:

**Setup**:
1. Make sure you have at least git 2.7 - [see ---recurse-submodules](https://github.com/blog/2094-new-year-new-git-release#new-configuration-setting-for---recurse-submodules)
2. Setup your config to push work in `traits.js` submodule: `git config push.recurseSubmodules traits.js`

**From here on after**
3. `cd traits.js` and do some work.
4. `git commit -am "[your message]"`
5. `git push` from `traits.js-website/`

If you do work in the `traits.js` submodule and **you can't use git 2.7** then you have to do all of this every time:
1. `cd traits.js`
2. Do work in `traits.js/`
3. `git commit -am "[your message]" && git push`
4. `cd ..`
5. `git commit traits.js -m "updated traits.js"`
6. `git push`
