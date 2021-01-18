# this is the dist folder of create-table-web-component with dummy table componenet 


this is added to package.json scripts

“build-my-comp”: “ng build --prod --single-bundle true --keep-polyfills”

then to build polyfills it was recommended in the blog [Creating framework-agnostic web components with Angular](https://medium.com/angular-in-depth/creating-framework-agnostic-web-components-with-angular-6cc6466d5c06)

ng g ngx-build-plus:wc-polyfill

it creates this in the dist folder,

Now cd to dist folder then add a package.json in it with 
this is compulsary,other details can also be added by doing  $ npm init 

{
    name:<name-of-pack>,
    version:<version-no>

}

this will produce tarball file (.tgz) which can be uploaded to npm via : $ npm publish 

In my case I took file create-table-1.0.0.tgz to the app in which I wantes to install it ,
then run

$ npm install create-table-1.0.0.tgz

import the 'create-table'  and use the <ce-table ><ce-table> element

