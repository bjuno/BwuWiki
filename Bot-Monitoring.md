
# Bot Monitoring

## 1. Creating a Discord Server

### Step 1: Create a Server
1. **Open Discord**: Log in to your Discord account.
2. **Click on the "+" button**: This is located on the left sidebar.
3. **Create a Server**:
   - Choose the option "Create My Own" or use a template.
   - Enter a server name.
   - Optionally, upload an icon for your server.
   - Click "Create".

### Step 2: Customize Your Server
1. **Create Channels**:
   - **Text Channels**: Click the "+" next to "Text Channels" to add channels (e.g., #general, #announcements).
   - **Voice Channels**: Click the "+" next to "Voice Channels" to add channels (e.g., General, Music).
   - **Categories**: Organize channels into categories by clicking the "+" next to the server name and selecting "Create Category".

2. **Set Up Roles**:
   - Go to "Server Settings" (click on your server name at the top and select "Server Settings").
   - Click on "Roles" and then the "+" button to create new roles.
   - Customize permissions for each role (e.g., Admin, Moderator, Member).
   - Assign roles to members by right-clicking on their username and selecting "Roles".

---

## 2. Setting Up "Auto Screenshot" Software

### Step 1: Download the Software
1. **Visit the Official GitHub repo**: Go to the [Auto Screenshot](https://github.com/artem78/AutoScreenshot) GitHub page.
3. **Download the Installer**: Scroll to the bottom and download for either Windows or Linux.

### Step 2: Configure Auto Screenshot
1. **Set Screenshot Intervals**: In the application settings, configure the intervals at which screenshots should be taken.
2. **Choose Save Location**: Select the folder where the screenshots will be saved.
3. **Adjust Capture Settings**: Configure additional settings like screen region, image format, and quality as needed.

### Step 3: Start Taking Screenshots
1. **Start the Service**: Click on the "Start" button within the application to begin automatic screenshot capture.
2. **Monitor Activity**: Ensure the application is running in the background to continuously capture screenshots at the set intervals.

---

## 3. Auto Upload to Discord Server Using DAU

### Step 1: Download the Software
1. **Visit the Official GitHub repo**: Go to the [DAU](https://github.com/tardisx/discord-auto-upload) GitHub page.
2. **Download the Installer**: Scroll to the bottom and download for either Windows or Linux.


### Step 2: Configure DAU
1. **Create a Configuration File**:
   - Create a new file named `config.json` in the `discord-auto-upload` directory.
   - Add the following configuration details:
     ```json
     {
       "discord_webhook_url": "YOUR_DISCORD_WEBHOOK_URL",
       "upload_interval": 60,
       "upload_directory": "path/to/screenshots"
     }
     ```
   - Replace `YOUR_DISCORD_WEBHOOK_URL` with the webhook URL of the Discord channel where you want to upload the screenshots.
   - Adjust the `upload_interval` to set how often (in seconds) the files should be uploaded.
   - Set the `upload_directory` to the folder where your screenshots are saved.

### Step 3: Run DAU
1. **Start the Script**:
   ```sh
   python dau.py
   ```
2. **Monitor Uploads**: Ensure that the script is running and check the Discord channel to confirm that the screenshots are being uploaded automatically.

By following these steps, you can set up automated screenshot capturing and uploading to your Discord server, making it easier to monitor activities and share updates with your community.
