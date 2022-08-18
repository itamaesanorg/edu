# Error Delete CR prettier.md

## For this situation

      mgarg@4746H MINGW64 /d/Repos/SushiJS-Example-01-1 (main)
      $ npm install

      > SushiJS-Boilerplate@1.7.2 postinstall
      > yarn husky install && yarn build

      yarn run v1.22.19
      $ D:\Repos\SushiJS-Example-01-1\node_modules\.bin\husky install
      husky - Git hooks installed
      Done in 0.15s.
      yarn run v1.22.19
      $ next build

      Failed to compile.

      ./pages/404.tsx
      1:29  Error: Delete `␍`  prettier/prettier
      2:1  Error: Delete `␍`  prettier/prettier
      3:40  Error: Delete `␍`  prettier/prettier
      4:1  Error: Delete `␍`  prettier/prettier
      5:37  Error: Delete `␍`  prettier/prettier
      6:11  Error: Delete `␍`  prettier/prettier
      7:34  Error: Delete `␍`  prettier/prettier
      8:110  Error: Delete `␍`  prettier/prettier
      9:103  Error: Delete `␍`  prettier/prettier
      10:79  Error: Delete `␍`  prettier/prettier
      11:48  Error: Delete `␍`  prettier/prettier
      12:14  Error: Delete `␍`  prettier/prettier
      13:51  Error: Delete `␍`  prettier/prettier
      14:60  Error: Delete `␍`  prettier/prettier
      15:71  Error: Delete `␍`  prettier/prettier
      16:80  Error: Delete `␍`  prettier/prettier
      17:81  Error: Delete `␍`  prettier/prettier
      18:75  Error: Delete `␍`  prettier/prettier
      19:15  Error: Delete `␍`  prettier/prettier
      20:56  Error: Delete `␍`  prettier/prettier
      21:138  Error: Delete `␍`  prettier/prettier
      22:41  Error: Delete `␍`  prettier/prettier
      23:17  Error: Delete `␍`  prettier/prettier
      24:18  Error: Delete `␍`  prettier/prettier
      25:26  Error: Delete `␍`  prettier/prettier
      26:138  Error: Delete `␍`  prettier/prettier
      27:27  Error: Delete `␍`  prettier/prettier
      28:17  Error: Delete `␍`  prettier/prettier
      29:18  Error: Delete `␍`  prettier/prettier
      30:15  Error: Delete `␍`  prettier/prettier
      31:13  Error: Delete `␍`  prettier/prettier
      32:17  Error: Delete `␍`  prettier/prettier
      33:4  Error: Delete `␍`  prettier/prettier
      34:2  Error: Delete `␍`  prettier/prettier
      
      [...]
      
      info  - Need to disable some ESLint rules? Learn more here: https://nextjs.org/docs/basic-features/eslint#disabling-rules
      error Command failed with exit code 1.
      info Visit https://yarnpkg.com/en/docs/cli/run for documentation about this command.    
      npm ERR! code 1
      npm ERR! path D:\Repos\SushiJS-Example-01-1
      npm ERR! command failed
      npm ERR! command C:\WINDOWS\system32\cmd.exe /d /s /c yarn husky install && yarn build  

      npm ERR! A complete log of this run can be found in:
      npm ERR!     C:\Users\mgarg\AppData\Local\npm-cache\_logs\2022-08-18T14_30_31_964Z-debug-0.log
      
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
