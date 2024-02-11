# jsdt1

**This is a personal project not intended for release**. There will be bugs and it's not feature-complete, but it served its purpose for me.

JSDT1 is a web-based editor for blocks as extracted using [Paul Siramy's DT1 Tools](http://paul.siramy.free.fr/), and then compiled back again using the same tool. Really it's just a UI for faster editing.

## "Install"

- Download the `/dist` folder.
- Install a local webserver, for instance:
  - [Web Server for Chrome](https://chromewebstore.google.com/detail/web-server-for-chrome/ofhbbkphhbklhfoeikjpcbhemlocgigb?hl=en) extension
  - [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension for VS Code
  - [http-server](https://www.npmjs.com/package/http-server) NPM package for node / JS
  - [http.server](https://docs.python.org/3/library/http.server.html#module-http.server) Python package
  - Any other local HTTP server
- Launch the `/dist` folder using this
- Go to `http://localhost:<your-port-here>`

## Usage

For the most part it should be _fairly_ self explanatory. There is also a `Help` subpage included in the app. Here is my use-case:

- Have a bunch of rendered images from [Blender D2Tools](https://github.com/muitdebos/blender-d2tools/tree/main/blender-d2tools)
- "Add New Empty BlocK" since we're creating an entirely new tileset
- On the left navigation bar go to FS (or whatever type of tile you want to do)
- In the toolbar, keep adding new blocks until you have as many as your total rendered images for this tile type.
- Repeat for other tile types.
- In the right column, "Image Library", import all images you want for this type.
- Hit "Apply All" to use use all these images in the blocks on the left. Make sure you have enough blocks for this.
- You can also manually click on a block on the left and select an image from the library.
- In the FS > Block Editor toolbar you can select the Grid icon. Then you can draw collision flags.
- Finally, go back to the INI tab and check to make sure all settings are as desired.
- Press "Save All", or any of the individual export options.
- Use the exported `.txt` blocklist and `.png` tilesheet with DT1 Tools.

## Tips

- You can export the INI as a CSV file which allows you to very quickly mass-edit Main / Sub indexes, and then import it back in to save as INI again.
- The X and Y of the tiles _should_ be handled automatically but the program is not 100% bugfree so either check or once you're done with manual changes, save everything and reimport everything in a clean refreshed page, type by type. This should almost certainly not cause issues.
- In WS / WD mode there is a `Mask` option that quickly masks out certain parts of the walls. It's optional and might save some time, but doesn't cover everything of course. But it's good enough for a first iteration before cleaning up the tilesheet in your image editor of choice.
- Not bugfree, try not to do too many crazy things at once.

Anything else, you can contact me on Discord, @Aerlynn#6848
