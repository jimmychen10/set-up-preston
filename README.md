# react-to-github-pages


## YouTube Tutorial Reference:

[How to Deploy a React App to GitHub Pages](https://www.youtube.com/watch?v=4G6O0BIoq6M)

## Steps:

0. After running `create-react-app`, extract all the files to the root directory.

1. Install GitHub Pages in your terminal:
    ```bash
    npm i gh-pages --save-dev
    ```

2. Go to `package.json` in your project folder.

3. Add the following line above the `"name"` key:
    ```json
    "homepage": "https://github_username_goes_here.github.io/",
    ```

4. Add deployment scripts to the `scripts` section in the `package.json` file

4.5. Example:
    ```json
    "scripts": {
        "predeploy": "npm run build",
        "deploy": "gh-pages -d build",
        "start": "react-scripts start",
        "build": "react-scripts build"
    }
    ```

5. Commit and push your changes.

6. Run the deployment command:
    ```bash
    npm run deploy
    ```

7. Watch the magic happen!


