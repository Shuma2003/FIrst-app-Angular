# FIrst-app-Angular
Step 1 - Test the default app
In this step, after you download the default starting app, you build the default Angular app. This confirms that your development environment has what you need to continue the tutorial.

In the Terminal pane of your IDE:

In your project directory, navigate to the first-app directory.

Run this command to install the dependencies needed to run the app.

content_copy
npm install
Run this command to build and serve the default app.

content_copy
ng serve
The app should build without errors.

In a web browser on your development computer, open http://localhost:4200.

Confirm that the default web site appears in the browser.

You can leave ng serve running as you complete the next steps.

Step 2 - Review the files in the project
In this step, you get to know the files that make up a default Angular app.

In the Explorer pane of your IDE:

In your project directory, navigate to the first-app directory.

Open the src directory to see these files.

In the file explorer, find the Angular app files (/src).

index.html is the app's top level HTML template.
style.css is the app's top level style sheet.
main.ts is where the app start running.
favicon.ico is the app's icon, just as you would find in any web site.
In the file explorer, find the Angular app's component files (/app).

app.component.ts is the source file that describes the app-root component. This is the top-level Angular component in the app. A component is the basic building block of an Angular application. The component description includes the component's code, HTML template, and styles, which can be described in this file, or in separate files.

In this app, the styles are in a separate file while the component's code and HTML template are in this file.

app.component.css is the style sheet for this component.

New components are added to this directory.

In the file explorer, find the image directory (/assets) that contains images used by the app.

In the file explorer, find the files and directories that an Angular app needs to build and run, but they are not files that you normally interact with.

.angular has files required to build the Angular app.
.e2e has files used to test the app.
.node_modules has the node.js packages that the app uses.
angular.json describes the Angular app to the app building tools.
package.json is used by npm (the node package manager) to run the finished app.
tsconfig.* are the files that describe the app's configuration to the TypeScript compiler.
After you have reviewed the files that make up an Angular app project, continue to the next step.

Step 3 - Create Hello World
In this step, you update the Angular project files to change the displayed content.

In your IDE:

Open first-app/src/index.html.

In index.html, replace the <title> element with this code to update the title of the app.

Replace in src/index.html
content_copy
<title>Homes</title>
Then, save the changes you just made to index.html.

Next, open first-app/src/app/app.component.ts.

In app.component.ts, in the @Component definition, replace the template line with this code to change the text in the app component.

Replace in src/app/app.component.ts
content_copy
template: `<h1>Hello world!</h1>`,
In app.component.ts, in the AppComponent class definition, replace the title line with this code to change the component title.

Replace in src/app/app.component.ts
content_copy
title = 'homes';
Then, save the changes you made to app.component.ts.

If you stopped the ng serve command from step 1, in the Terminal window of your IDE, run ng serve again.

Open your browser and navigate to localhost:4200 and confirm that the app builds without error and displays Hello world in the title and body of your app:

browser frame of page displaying the text 'Hello World'
Lesson review
In this lesson, you updated a default Angular app to display Hello world. In the process, you learned about the ng serve command to serve your app locally for testing.

If you have any trouble with this lesson, review the completed code for it in the live example / download example.
