# Test Passing parameters to a sketch plugin

The goal of this repository is to get a working example of passing parameters to sketch plugin from the command line. This was created to work against the sketch43 beta.

To install plugin place "ContextTest.sketchplugin" in your plugin directory: 
  ```
  ~/Library/Application Support/com.bohemiancoding.sketch3/Plugins
  ```

Invoking the sketch plugin:
  ```
  ./run.sh
  ```

Or without the shell script:
  ```
  /Applications/Sketch\ Beta.app/Contents/Resources/sketchtool/bin/sketchtool run ~/Library/Application\ Support/com.bohemiancoding.sketch3/Plugins/ContextTest.sketchplugin contextTest --context='{ "x": 2 }'
  ```

Output of run:
  ```
  context: {
      api = "<MOJavaScriptObject: 0x61800022b300>";
      command = "<MSPluginCommand: 0x6100000efc80>";
      document = "<MSDocument: 0x7f9d3175b1c0>";
      plugin = "<MSPluginBundle: 0x6100000fe700>";
      scriptPath = "/Users/joekim/Library/Application Support/com.bohemiancoding.sketch3/Plugins/ContextTest.sketchplugin/Contents/Sketch/run.js";
      scriptURL = "file:///Users/joekim/Library/Application%20Support/com.bohemiancoding.sketch3/Plugins/ContextTest.sketchplugin/Contents/Sketch/run.js";
      selection =     (
      );
  }
  context.x: null
  ```  
