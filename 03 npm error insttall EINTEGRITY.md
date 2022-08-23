Scenario: Trying to install from npm any package, I got this error:
![npm error insttall EINTEGRITY](https://user-images.githubusercontent.com/5947268/186204815-256978f2-eb8a-4fbc-a768-0891f0775534.png)

Solution: To solve this I execute:
       rm -rf package-lock.json node_modules

Then:
        npm install

Credits: 
[Das_Geek](https://stackoverflow.com/users/11384392/das-geek)
[Kodali444](https://stackoverflow.com/users/5168242/kodali444)

From:
[Fix a npm install failure with error code EINTEGRITY](https://stackoverflow.com/questions/49092723/fix-a-npm-install-failure-with-error-code-eintegrity)

Related with:
SUSHIJS ✅ FIXED from npm i sushis
SUSHIJS BOILERPLATE ✅ FIXED from npm i sushis-demo
