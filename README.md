# Bing AI Plugin

The Bing AI Plugin enables Auto-GPT to use Bing AI to research information, ask questions, get advice, and more.

<img width="1063" alt="Screenshot 2023-05-01 at 7 49 55 AM" src="https://user-images.githubusercontent.com/107640947/235470972-792b83ec-11a0-418f-88d3-33ef9fb116b2.png">

## Key Features:
- Bing AI already implemented researching information, so implementing this plugin will almost entirely negate the need to browse websites and the current implementation of researching information.
- Allows Auto-GPT to consult Bing AI.
- Allows Auto-GPT to be able to use GPT-4 as Bing AI is based on GPT-4.
- Brings GPT-4 functionality to those without GPT-4 API access.

## Getting Authentication (Required):
- Install the cookie editor extension for [Chrome](https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm) or [Firefox](https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/)
- Go to `bing.com`
- Open the extension
- You must be logged in to an account with Bing AI access.
- Click "Export" on the bottom right, then "Export as JSON" (This saves your cookies to clipboard)
- Paste your cookies into a file `cookies.json`
- IMPORTANT: Move the `cookies.json` file into the Auto-GPT folder.

## Installation

Follow these steps to configure the AutoGPT Bing AI Plugin:

### 1. Clone this Repository
cd into a folder that you can find easily. For example: `cd desktop`. 
Then, paste this command: `git clone https://github.com/gravelBridge/AutoGPTBingAI.git`

### 2. Navigate to the folder
Navigate to the folder where you ran the cd command

### 3. Zip the BingAI folder
On MacOS, right click the BingAI folder and press `Compress`. On windows, right click the folder, and press `Send to > Compressed (zipped)`.

### 4. Move the zip file
Move the new BingAI.zip file to the AutoGPT plugins directory, there should already be a file there titled `__PUT_PLUGIN_ZIPS_HERE__`.

### 6. Add BingAI configuration settings
Append the following configuration settings to the end of the .env file:

```ini
################################################################################
### BINGAI
################################################################################

BINGAI_COOKIES_PATH=./cookies.json
```

## AutoGPT Configuration
Set `ALLOWLISTED_PLUGINS=BingAI,example-plugin1,example-plugin2,etc` in your AutoGPT `.env` file.


### 7. Edit goals
When using Auto-GPT please set one of the goals to "Use ask_bing_genius whenever possible".
