Ionic Three.js Custom Component
===============================
Leon Battista Alberti in 1467 described cipher disk. 
This is a sample Ionic App with custom CypherComponent based on Three.js.

Install Node dependencies
------------------------

    $ npm install

Running
-------

Local browser:

    $ ionic serve


Create your own custom app
--------------------------

Ensure you have node, npm and ionic installed and updated.

Then, create a new App and add Three.js as a dependency:

```
$ ionic start my-app
$ cd my-app
$ npm install three --save
$ npm install @types/three --save-dev
```

Copy components/cypher folder to your components folder

```
$ cp -R components/cypher [your components folder]
```

Add <cypher-screen> tag where you want to include the CypherComponent component:

```html
<ion-content>
  <div style="width:100%; height:100%"> 
    <cypher-screen></cypher-screen>
  </div>
</ion-content>
```

Modify your app.module.ts file as the following:
Edit your app.module.ts adding `CypherComponent` component to your declarations section:
```javascript
import { CypherComponent } from '../components/cypher/cypher';

@NgModule({
  declarations: [

    CypherComponent
  ],

```
Run your project with and enjoy your 3D scenes:

```
$ ionic serve
```

