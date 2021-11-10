Steps to create this site:

```
brew install hugo
hugo new site learn-demo
cd learn-demo
git init
git submodule add https://github.com/cntrump/hugo-notepadium.git themes/notepadium
echo theme = \"notepadium\" >> config.toml
hugo new _index.md
hugo new posts/my-first-post.md
hugo new posts/my-second-post.md
hugo server -D
```

Then edit the posts, remove the `draft: true` from the post metadata.

Commit all these changes.

Create a repo on GitHub and push to it.

To configure with Netlify, do the following:

1. Log in
1. Click "New site from Git"
1. Authorize GitHub and select your repo
1. Take all the defaults to deploy
1. Wait for a minute and view the site at the generated URL

Make a change locally, commit and push, verify that Netlify runs a new deployment with the changeso
