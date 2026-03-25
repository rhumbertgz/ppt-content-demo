
## Run the sample

### Run the sample with GitHub as the host

An Office Add-in requires you to configure a web server to provide all the resources, such as HTML, image, and JavaScript files. The Hello World sample is configured so that the files are hosted directly from this GitHub repo, so all you need to do is build the manifest and package, and then sideload the package.

1. Clone or download this sample to a folder on your computer. Then in a command prompt, bash shell, or **TERMINAL** in Visual Studio Code, navigate to the root of the sample folder.
1. Run the command `npm install`.
1. Run the command `npm run build`.
1. Run the command `npm run start:prod`.

   After a few seconds, desktop PowerPoint opens, and after a few seconds more, the content add-in appears over the current slide with a **Get slide details** button.
     - If the content add-in doesn't appear, use the **Add-ins** button in the **Home** tab of the ribbon, then select the name of the content add-in, "PowerPoint Content Add-in".

1. Choose the **Get slide details** button to display "Hello, world!" and slide details.
1. To try this out in PowerPoint on the web:
   1. Open a presentation.
   1. Use the **Add-ins** button in the **Home** tab of the ribbon, then select the name of the content add-in, "PowerPoint Content Add-in". If the add-in is absent, select the **Manage** link then open the add-in from there.

When you're finished working with the add-in, close PowerPoint, and then in the window where you ran the three npm commands, run `npm run stop:prod`.

### Configure a localhost web server and run the sample from localhost

If you prefer to configure a web server and host the add-in's web files from your computer, use the following steps.

1. Clone or download this sample to a folder on your computer. Then in a command prompt, bash shell, or **TERMINAL** in Visual Studio Code, navigate to the root of the sample folder.
1. Run the command `npm install`.
1. Run the command `npm start`.

   - If you've never developed an Office Add-in on this computer before or it has been more than 30 days since you last did, you'll be prompted to delete an old security cert and/or install a new one. Agree to both prompts.
   - After a few seconds, a **webpack** dev-server window will open and your files will be hosted there on localhost:3000.
   - When the server is successfully running, desktop PowerPoint opens, and after a few seconds more, the content add-in appears over the current slide with a **Get slide details** button.
     - If the content add-in doesn't appear, use the **Add-ins** button in the **Home** tab of the ribbon, then select the name of the content add-in, "PowerPoint Content Add-in".

1. Choose the **Get slide details** button to display "Hello, world!" and slide details.
1. To try this out in PowerPoint on the web:
   1. Open a presentation.
   1. Use the **Add-ins** button in the **Home** tab of the ribbon, then select the name of the content add-in, "PowerPoint Content Add-in". If the add-in is absent, select the **Manage** link then open the add-in from there.
      - **Note**: Depending on your machine's network or security settings, the add-in's web conent might not be accessible.

When you're finished working with the add-in, close PowerPoint, and then in the window where you ran the two npm commands, run `npm stop`.
