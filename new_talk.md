
## Instructions to make a new talk

1. Create a new branch with a folder for the new talk
```
git checkout -b new_talk
cp -a template/ new_talk/ && cd new_talk/
```

2. Add reveal.js

If you nead the `darkenergy` theme:
```
git submodule add https://github.com/EiffL/reveal.js.git
```

Else:
```
git submodule add https://github.com/hakimel/reveal.js.git
```

Then update it and copy the files needed to start your own `index.html`
```
cd reveal.js
git submodule update --init --recursive
cd ..
cp reveal.js/gulpfile.js .
cp reveal.js/package.json .
```

3. Launch the server
```
npm install
npm start
```