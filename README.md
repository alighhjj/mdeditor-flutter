# Markdown Editor - Flutter

This is a Markdown editor application built with Flutter. It features a real-time preview of Markdown text as you type with a responsive layout that adapts to different screen sizes.

## Features

- Split-screen editor with real-time preview
- Support for all common Markdown syntax including images
- Responsive design:
  - Left/right layout on PC screens (width > 800px)
  - Top/bottom layout on mobile screens
- Syntax highlighting for code blocks
- Beautiful UI with shadows and rounded corners
- Custom styling for different Markdown elements

## Setup

1. Clone this repository

2. Install Flutter dependencies:
   ```
   flutter pub get
   ```

3. Run the app:
   ```
   ./run.sh
   ```

4. Open your browser to the URL provided (typically http://localhost:3000)

## Layout

The application features a responsive design that automatically adapts to different screen sizes:
- On PC screens (width > 800px): Left/right layout with editor on the left and preview on the right
- On mobile screens: Top/bottom layout with editor on top and preview at the bottom

## Usage

1. Type Markdown in the editor pane
2. See the rendered output in the preview pane in real-time
3. The editor comes pre-loaded with example Markdown to help you get started
4. To preview images, use the standard Markdown syntax: `![alt text](image_url)`

## Development

This project is set up to work with GitHub Codespaces, making it easy to develop directly in your browser. Follow the original instructions in the section below if you want to use Codespaces.

## Original Codespaces Instructions

<details>
<summary>Click here to see the original Codespaces setup instructions</summary>

### Important things to note

Codespaces is not completely free. Free users have 120 core-hours per month and Pro users have 180 core-hours per month. The default codespace runs on a 2-core machine, so that's 60 hours (or 90 hours) of free usage per month before getting charged. Make sure to stop your codespace when you're not using it (it automatically stops after 30 minutes of inactivity by default). See more pricing details [here](https://docs.github.com/en/billing/managing-billing-for-github-codespaces/about-billing-for-github-codespaces), and manage your active codespaces [here](https://github.com/codespaces).

### Getting started

1. Press "Use this template" towards the top right of this repository and create a new repository from this template.

    > There's also an option to open this repository in Codespaces and publish it to GitHub later from there, but I recommend creating your own repository first.

2. In your new repository, press "Code", select "Codespaces", then press "Create codespace on main". A container with everything you need to get started will be created automatically, then you'll be taken to your new codespace (VS Code in your browser). If you'd prefer to work on your codespace using the VS Code desktop app instead of the browser app, you can follow these instructions.

3. Press the "Extensions" icon in the left sidebar. You'll see that the Flutter and Dart extensions are already being installed. The environment won't work properly until the installation is complete, so wait for it to finish.

4. In your integrated terminal (the TERMINAL tab), run `flutter pub get` to install the missing Flutter dependencies.

5. In the ports view (the PORTS tab), port 3000 should be listed there already. Right click on it, and, under "Port Visibility", select "Public". This is important so the app can access services on your client from other server ports without getting blocked due to CORS.

6. Run `./run.sh` in the terminal to start the app. A notification will appear saying that an app opened on port 3000. You can press "Open in Browser" to open it, but it won't load until the terminal shows that it's ready. You can refresh once the app is loaded (as indicated by a prompt to press "R" to reload).

    > You can find the link to access the app in your browser at any time by going to the ports view, right clicking on port 3000, and pressing "Open in Browser".

7. That's it! Make changes in `lib/main.dart`, press "R" in the terminal, then refresh the page to see your changes appear quickly.

### Using a sample

There are a collection of sample Flutter apps you can use. They're stored in the `samples` directory. If you want to use one of them, find the folder of the sample you want to use, then move the contents of the folder into the root of your repository. At minimum, this should overwrite `pubspec.yaml` and `lib`.

### Development Environment

#### Developing in the browser

The browser-based VS Code is the default editor for Codespaces, and has most of the features you'd need. Opening your codespace from [github.com/codespaces](https://github.com/codespaces) will automatically open the browser-based editor.

#### Developing in the desktop app

If you'd prefer to use the desktop app version of VS Code, you can follow these instructions:

1. Download the [VS Code desktop app](https://code.visualstudio.com/). You probably already have it if you chose to follow these instructions.

2. Install the [GitHub Codespaces extension](https://marketplace.visualstudio.com/items?itemName=GitHub.codespaces).

3. Open the command pallette from the View menu (or cmd+shift+P / ctrl+shift+P) and run "Codespaces: Connect to Codespace...".

    > Alternatively, click the button in the very bottom left of VS Code (it says "Open a Remote Window" if you hover over it) and press "Connect to Codespace...".

4. Log in if necessary, then select your codespace from the list.

### Flutter Development

#### Developing for mobile

Running Flutter in Codespaces makes it a bit difficult to run the app in a mobile simulator. However, developing for the web is basically the same as developing for mobile. I'd recommend opening your browser's developer tools and selecting a mobile device to emulate.

If you're using Chrome or another Chromium-based browser, you can open DevTools like [this](https://developer.chrome.com/docs/devtools/open/) and emulate a device like [this](https://developer.chrome.com/docs/devtools/device-mode/). It'll be pretty similar for other browsers like Safari and Firefox.

### Codespaces Usage

#### Managing your codespace

When you're not using your codespace, deactivate it by going to [Codespaces](https://github.com/codespaces), pressing the 3 dots on the right side of the codespace, and pressing "Stop codespace". You can also deactivate it within the codespace by pressing "Codespaces" at the bottom left of VS Code and selecting "Stop Current Codespace".

Edited files in your workspace are not deleted when stopping the codespace and the container won't need to be rebuilt when you start it again. Provided that you're under the storage limit (15 GB for Free users and 20 GB for Pro), you won't be charged if your codespace is offline. I recommend committing your repository changes on your codespace often to avoid losing work if you were to delete your codespace.

</details>
