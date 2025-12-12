## Scope of the project
This project exists to create, update, and share Starter Guides that help university students through the installation of required software, answer frequently asked questions, and streamline the resolution of common issues encountered in these processes.

## Recommended practices for collaborators

### General conventions
- Write clear, meaningful commit messages that describe what was changed and why.
- Prefer small, focused commits over large, mixed ones.

### Project structure and assets
- For each guide, place all images in the `Images` directory inside that guide’s root folder.
- When creating a new LaTeX file for a guide, set the graphics path to the `Images` directory of that guide and follow the existing folder naming conventions.
- Do not store images or other assets directly next to the `.tex` files if an `Images` directory exists.

### Compilation and build artifacts
- Prefer compiling each guide into a `Build` subfolder inside that guide’s directory, so that intermediate LaTeX files are automatically ignored according to the `.gitignore`.
- If you compile in the guide’s root directory instead of `Build`, be aware that some intermediate files may still be ignored by the redundant patterns in `.gitignore`, but keeping everything in `Build` is strongly recommended.
- Avoid committing temporary or editor-specific files; if needed, update `.gitignore` rather than adding such files to version control.

### Compiled guides
- After updating a guide, compile it and place the resulting PDF into the `CompiledGuides` folder so that the final versions are easy to find and ready to distribute.
- The guides inside `CompiledGuides` are considered "ready to distribute" versions, so please don't replace the .pdf guide in there with an unfinished version.
- Keep the `CompiledGuides` folder organized by using the name of the `.tex` file as the name of the guide and replace the old version with the new one when updating them.
