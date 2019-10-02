## Explanation of Ionic for correcting if not familair with the framwork

Ionic apps are built with Cordova. Cordova is a means of packaging html/css/js into apps that can run on mobile and desktop devices and provides a plugin architecture for accessing native functionality beyond the reach of JS run from a web browser. As such, Ionic apps have the Cordova file structure. Ionic project is built on Angular with the help of node js too.
### ./src/
Inside of the src directory we find our code. This is where most of the work for an Ionic app will take place. When we run ionic serve, our code inside of src/ is transpiled into the correct Javascript version that the browser understands (currently, ES5). That means we can work at a higher level using TypeScript, but compile down to the older form of Javascript the browser needs.

src/app/app.module.ts is the entry point for our app.

Every app has a root module that essentially controls the rest of the application.

In this module, we’re setting the root component to MyApp, in src/app/app.component.ts. This is the first component that gets loaded in our app, and typically it’s an empty shell for other components to be loaded into. In app.component.ts, we’re setting our template to src/app/app.html

### Pages
The contents of src/pages/ shows all of our pages of our hybrid application.