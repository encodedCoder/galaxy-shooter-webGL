# Galaxy Shooter

Galaxy Shooter is a Unity WebGL game that can be played directly in a web browser. This project contains the necessary files to run the game on GitHub Pages.

## Project Structure

```
Build/
    ├── WebGL Demo.data.unityweb
    ├── WebGL Demo.framework.js.unityweb
    ├── WebGL Demo.loader.js
    ├── WebGL Demo.wasm.unityweb
index.html
TemplateData/
style.css
```

## Deployment

To deploy this game on GitHub Pages, follow these steps:

1. **Create a GitHub Repository**:

   - Go to GitHub and create a new repository.
   - Clone the repository to your local machine.

2. **Copy Your Project Files**:

   - Copy the entire contents of your project (including `Build`, `TemplateData`, and `index.html`) into the cloned repository directory.

3. **Commit and Push**:

   - Commit the changes and push them to the GitHub repository.

   ```sh
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```

4. **Enable GitHub Pages:**

   - Go to the repository settings on GitHub.
   - Scroll down to the "GitHub Pages" section.
   - Select the branch you want to deploy from (usually main) and the root directory (/).
   - Save the settings.

5. **Access Your Game:**
   - After a few minutes, your game should be accessible at `https://encodedcoder.github.io/galaxy-shooter-webGL/`.

## Important Considerations

- **File Paths:** Ensure that all file paths in your `index.html` are relative and correctly point to the `Build` and `TemplateData` directories.
- **Case Sensitivity:** GitHub Pages is case-sensitive, so make sure the file names and paths match exactly.

## How It Works

1. **HTML Setup:** The `index.html` file sets up the HTML structure, including a canvas element where the Unity game will be rendered.
2. **Loading Unity:** The `WebGL Demo.loader.js` script is loaded, which initializes the Unity instance and starts loading the game's data, framework, and WebAssembly files.
3. **Progress Display:** The loading progress is displayed using a progress bar.
4. **Game Initialization:** Once all necessary files are loaded, the Unity instance is created, and the game starts running in the canvas element.
5. **Fullscreen and Warnings:** The script also handles fullscreen functionality and displays warnings or errors if any issues occur during loading.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgements

- Unity Technologies for providing the Unity engine.
- Bootstrap for the responsive design framework.
- jQuery and Popper.js for additional JavaScript functionality.

## Author

Suresh

Enjoy playing Galaxy Shooter!
