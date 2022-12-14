# bgEditor

Authors: Phil Kanaby, ok

See editor documentation in [docs/editor_docs.txt](./docs/editor_docs.txt)

## Running

### IntelliJ IDEA

1. Import this project into IntelliJ IDEA as a Maven project
2. Click the refresh icon on top right of the editor panel
3. On the right, click "Maven" then "Lifecycle" then "package"
4. Create a new run configuration on the top right with it being an "Application"
5. Name it "Editor" and click "Modify Options" and "Add JVM options"
6. Set the JVM options to `-Xmx3G -Xms3G -XX:+UseParallelGC`.
   - *Bob said you likely need 16GB ram to use it for big maps.*
7. Set the main class to `com.bobsgame.EditorMain`
8. Apply then click "OK"
![Run Configuration](./docs/run_configuration.png)
9. Click the run button on the top right and the editor will open.

### Eclipse
1. Load the project as a Maven project.
2. Run "package" Maven task.
3. Run.

## Building 

1. Import this project into IntelliJ IDEA as a Maven project
2. Click the refresh icon on top right of the editor panel
3. On the right, click "Maven" then "Lifecycle" then "package"
4. The final, shaded jar will be in `target/bgEditor-shaded-<VERSION>.jar`

## Exporting the Map

1. Clone the okWorldAssets repo from https://github.com/bobsgamed/okWorldAssets.git
2. Go to your editor and head to File > Open Project
3. Open the zip file in okWorldAssets
4. Wait a few minutes while the maps load.
5. Click on File > Export Project To ...
6. You may get a lot of errors informing you that sfx and bgm are missing. Don't worry about this right now as it still exported.
7. Exit via File > Exit (no autosave)
