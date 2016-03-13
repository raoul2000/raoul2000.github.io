This branch is the hexo source files

## Prepare working copy

```
git clone -b hexo-source --single-branch https://github.com/raoul2000/raoul2000.github.io.git
cd raoul2000.github.io
npm install
```

## Work with Hexo

- create a post : `hexo new "My New Post"`
- run server : `npm run server`
- generate static files : `hexo generate`

## Update site
The command `hexo generate` produces files into the *public* folder. These files are the source file of the blog and therefore must be pushed to the **master** branch.

To do so, use command :
```
hexo deploy
```
(*see configuration file `_config.yml` section "deploy"*)

This command creates folder `.deploy_git` which contains a copy of the *public* files that were pushed to master branch.

## Save source

Before pushing changes to the *hexo-source* branch, make sure that new post are committed !

```
git status
git add source/**
git commit -a -m "commit message"
```

Finally push to origin :

```
 git push origin hexo-source
```
