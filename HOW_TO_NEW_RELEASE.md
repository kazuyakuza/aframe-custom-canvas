1- modify in package.json:
1.a- the "version" property value
1.b- the script "prerelease" property. You should replace older version with current, and current with new version:
--> from "node scripts/release.js 1.2.3 1.2.4"
--> to "node scripts/release.js 1.2.4 1.2.5"
2- PR and merge your changes
3- check dependencies are installed `npm i`
4- build the new dist `npm run dist`
5- updates dist files for release `npm run prerelease`
6- verify you are correctly logged `npm whoami`
7- publish the new release `npm publish`
8- PR & merge release changes
