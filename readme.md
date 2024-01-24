# Multi (PlatformIO) Project

This Project / VSCode Workspace is intended as Template for one git repository that holds multiple PlatformIO or other independent Projects.

Subfolders `project1` and `project2` are just regular project folders without any special files or structure. In this example, they are Platform IO Projects, each containing a `platformio.ini`.

The "magic" happens in the `projects.code-workspace` file. It maps the subfolder `project1` and `project2` into top-level folders, enabling PlatformIO (or other extensions) for them in VSCode. Folders can optionally be renamed for better structuring. Also the root Folder `.` is mapped into `main` so all other files that are not part of the project folders, like this readme, can be edited. Folder `project1` is hidden from the `main` folder though, via `.vscode/settings.json`.