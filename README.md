#SVG drawing and animation using TweenMax

Here you can find how to create dynamics paths into SVG tag, storing all coordinates in a simple array.
For this example, I needed to create a HTML element using NS for use in SVG tag, some like this:

```
let createPath = document.createElementNS(NS,'path');
createPath.setAttribute('class', 'line');
createPath.setAttribute('d', line);
```
We should assign the class name instead through `setAttribute` because using `.classList.add` Internet Explorer take the path as a simple string, not as coordinate path.
Check the function on `index.js` file.

#Run project

Install npm modules 
<br>
`npm install`

Then, install `parcel` to bundle the files 
<br>
`npm install -g parcel-bundler`

More details in parcel oficial site.

#Run local server and compile the files
`npm run dev`