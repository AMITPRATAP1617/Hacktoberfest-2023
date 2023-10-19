The provided `manifest.json` file and `Content.js` script are for creating a Chrome extension that blocks access to specific social media websites and displays a custom error page when the user tries to access those sites.

Here's a brief overview of how the code works:

### `manifest.json`:
- `manifest_version`: Specifies the version of the manifest file format.
- `name`: Name of the Chrome extension ("Social Media Blocker").
- `version`: Version number of the extension.
- `content_scripts`: Specifies the content script (`Content.js`) and the URLs (`<all_urls>`) where the script will run.
- `icons`: Icon for the extension displayed in the browser toolbar.

### `Content.js`:
- The `generateSTYLES` function generates CSS styles for the custom error page.
- The `generateHTML` function generates the HTML content for the error page based on the social media site being blocked.
- The `switch` statement checks the current URL and replaces the document's head and body content with the custom styles and error message accordingly.

### Prerequisites:
- You need to have Google Chrome or a Chromium-based browser installed on your system to load and test the extension.

### How to Run the Program (Chrome Extension):
1. **Create a Folder**: Create a folder on your computer to store the extension files.

2. **Add Files**: Inside the folder, create two files: `manifest.json` and `Content.js`. Copy the respective code into each file.

3. **Load Extension in Chrome**:
   - Open Chrome.
   - Go to `chrome://extensions/`.
   - Enable "Developer mode" (usually a toggle switch at the bottom).
   - Click on "Load unpacked."
   - Select the folder where your extension files (`manifest.json` and `Content.js`) are located.

4. **Test the Extension**:
   - Visit a social media site like YouTube, Facebook, Instagram, Twitter, or Netflix.
   - The extension should block access to these sites and display a custom error message.

Please note that this extension will only work when the website URLs match the patterns specified in the `switch` statement. You can modify the `switch` statement to add or remove social media sites as needed.

Additionally, always be cautious when running browser extensions, especially those that modify web content, as they can potentially compromise your online security and privacy.

Contact Details:
Github: Shashi3k
X: @Shashi3k
