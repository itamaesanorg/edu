# Error Delete CR prettier.md

## For this situation

      user@mbp /c/somewhere/Project(main)
      $ npm install

      > SushiJS-Boilerplate@1.7.2 postinstall
      > yarn husky install && yarn build

      yarn run v1.22.19
      $ D:\somewhere\SushiJS-Example-01-1\node_modules\.bin\husky install
      husky - Git hooks installed
      Done in 0.15s.
      yarn run v1.22.19
      $ next build

      Failed to compile.

      ./pages/404.tsx
      1:29Error: Delete `␍`prettier/prettier
      2:1Error: Delete `␍`prettier/prettier
      3:40Error: Delete `␍`prettier/prettier
      4:1Error: Delete `␍`prettier/prettier
      5:37Error: Delete `␍`prettier/prettier
      6:11Error: Delete `␍`prettier/prettier
      7:34Error: Delete `␍`prettier/prettier
      8:110Error: Delete `␍`prettier/prettier
      9:103Error: Delete `␍`prettier/prettier
      10:79Error: Delete `␍`prettier/prettier
      11:48Error: Delete `␍`prettier/prettier
      12:14Error: Delete `␍`prettier/prettier
      13:51Error: Delete `␍`prettier/prettier
      14:60Error: Delete `␍`prettier/prettier
      15:71Error: Delete `␍`prettier/prettier
      16:80Error: Delete `␍`prettier/prettier
      17:81Error: Delete `␍`prettier/prettier
      18:75Error: Delete `␍`prettier/prettier
      19:15Error: Delete `␍`prettier/prettier
      20:56Error: Delete `␍`prettier/prettier
      21:138Error: Delete `␍`prettier/prettier
      22:41Error: Delete `␍`prettier/prettier
      23:17Error: Delete `␍`prettier/prettier
      24:18Error: Delete `␍`prettier/prettier
      25:26Error: Delete `␍`prettier/prettier
      26:138Error: Delete `␍`prettier/prettier
      27:27Error: Delete `␍`prettier/prettier
      28:17Error: Delete `␍`prettier/prettier
      29:18Error: Delete `␍`prettier/prettier
      30:15Error: Delete `␍`prettier/prettier
      31:13Error: Delete `␍`prettier/prettier
      32:17Error: Delete `␍`prettier/prettier
      33:4Error: Delete `␍`prettier/prettier
      34:2Error: Delete `␍`prettier/prettier

      [...]

      info- Need to disable some ESLint rules? Learn more here: https://nextjs.org/docs/basic-features/eslint#disabling-rules
      error Command failed with exit code 1.
      info Visit https://yarnpkg.com/en/docs/cli/run for documentation about this command.
      npm ERR! code 1
      npm ERR! path D:\somewhere\SushiJS-Example-01-1
      npm ERR! command failed
      npm ERR! command C:\WINDOWS\system32\cmd.exe /d /s /c yarn husky install && yarn build

      npm ERR! A complete log of this run can be found in:
      npm ERR! C:\Users\user\AppData\Local\npm-cache\_logs\2022-08-18T14_30_31_964Z-debug-0.log
      
## Use

     For a newbie like me, this is how it is to be done. Open .eslintrc.json present in your root directory (frontend). After changes it will look as under: {   "extends": ["react-app", "prettier"],   "plugins": ["prettier"],   "rules": {     "prettier/prettier": ["error", { "endOfLine": "auto" }]   } } 
Source: https://stackoverflow.com/questions/53516594/why-do-i-keep-getting-delete-cr-prettier-prettier

## Instructions
###Instructions for SushiJS, on source project folder we added:
      .eslintrc.json
and typed:
{   "extends": ["react-app", "prettier"],   "plugins": ["prettier"],   "rules": {     "prettier/prettier": ["error", { "endOfLine": "auto" }]   } }

## Credits
Thanks to: Author: https://stackoverflow.com/users/3722884/simpleguy
