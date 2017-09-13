# NodeBox code sketches

This is basic flow/way to build your own automated interface for code sketches utilising gitHub pages.

Details in this medium article: 

There's just one setting you need to update in the `index.html`, your repo name (around `line 73`), where the render code is (be sure to include the branch). The other option is how may columns you prefer in the webpage (it uses [flex grid](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Using_CSS_flexible_boxes))

``` js
settings: {
    githubUrl: 'https://github.com/eesur/nodebox-daily-sketches/tree/master/',
    columns: 3
}
```


-----------

## setup

prerequisites: 
- [node](https://nodejs.org/en/) installed
- git installed

in your terminal:

0. [clone](https://help.github.com/articles/cloning-a-repository/) this repo to your computer (without the history): `git clone https://github.com/eesur/nodebox-daily-sketches.git && rm -rf nodebox-daily-sketches/.git`
1. run `npm update` to install `package.json` dependencies
2. delete the sketches and code, within and add your own
3. create your repo and push to it
4. set up gitHub Pages (just go to setting tab in your repo and turn on github pages)

-----------

## use

### 01. Add your files
- Save your NodeBox file into the `code` folder
- For each sketch export a `png` image into the `img-ref` folder

**NOTE:** Make sure you name the `code` files and `img` files the same, for example in this template I've named the images `[number-name].png/gif` and the code `[number-name].ndbx`

### 02. Update
- Update the data in the files: `run npm tree` 
- push


-----------

## breakdown of folders/files

- `code`: is a folder containing the code files
- `img-refs`: folder for all the images (png and gif)
- `directory-tree.js`: is the folder structure of the code files
- `imgTee.json`: is the folder structure of the image folders
