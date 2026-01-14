
## Instruction to make a new talk

```
git checkout -b new_talk
mkdir new_talk && cd new_talk
git submodule add https://github.com/hakimel/reveal.js.git
cd reveal.js
git submodule update --init --recursive
cd ..
cp reveal.js/gulpfile.js .
cp reveal.js/package.json .
npm install
npm start
```