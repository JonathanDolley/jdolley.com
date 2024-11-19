# Site set up

1. hugo new site ./ --formal=yaml --force
2. hugo mod init github.com/JonathanDolley/jdolley.com
3. Add module section to hugo.yaml file:


module:
  imports:
  - path: github.com/hugo-toha/toha/v4
  mounts:
  - source: ./node_modules/flag-icon-css/flags
    target: static/flags
  - source: ./node_modules/@fontsource/mulish/files
    target: static/files
  - source: ./node_modules/katex/dist/fonts
    target: static/fonts

4. hugo mod get -u
5. hugo mod tidy
6. hugo mod npm pack
7. npm install

