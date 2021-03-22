## Creating your own module
 - Choose what type of module do you want to make? [List of module types](home.md#what-is-a-module)
 - Create a new project on android studio
 - Clone the [openblocks-module-interface](github.com/OpenBlocksTeam/openblocks-module-interface) library
 - Right click the `app` module, hover over "New" and click "Module"
 - Click "Import Gradle Project"
 - Navigate to the folder where you cloned openblocks-module-interface
 - Check the Import checkbox
 - Name the module `module-interface`, or you can pick your own, this doesn't matter
 - Then click Ok
 - Remove `MainActivity.java` and `activity_main.xml` on your `app` module
 - Create a new java file and set the class to extend one of OpenBlocksModule's sub-interfaces, example:
   ```java linenums="1"
   public class MyModule implements OpenBlocksModule.ProjectManager {
   ```
 - Hit Alt+Shift+Enter to implement the methods
 - Click Ok
 - Start coding ;)

## Compiling module
- Compile it as an APK (Build > Build Bundles/APK > Build APK)
- Rename the APK extension to be a JAR file
- Create a file named `openblocks-module-manifest.json`, edit and put this code:
```json linenums="1"
{
    "name": "MyModule",
    "description": "My awesome OpenBlocks module",
    "classpath": "com.openblocks.module.MyModule",
    "version": 1,
    "lib_version": 1,
    "type": "PROJECT_MANAGER"
}
```
- Zip all of those files (JAR, and the `openblocks-module-manifest.json`) into 1 zip file
- Finally, Import it on the OpenBlocks App

## Examples
We've made default modules for our app, you might want to use them as your example


 - Project Manager: [ezmanager](https://github.com/OpenBlocksTeam/ezmanager)
 - Project Parser: [open-parsh](https://github.com/OpenBlocksTeam/open-parsh)
 - Project Code GUI & Blocks Collection: Coming soon
 - Project Layout GUI: Coming soon
 - Project Compiler: [mora-compiler](https://github.com/OpenBlocksTeam/mora-compiler)


More information: [https://stackoverflow.com/a/25748704/9613353](https://stackoverflow.com/a/25748704/9613353), [https://stackoverflow.com/a/6860579/9613353](https://stackoverflow.com/a/6860579/9613353)
