<h1 align="center">kudos-gpt</h1>

<h4 align="center">
  <a href="https://github.com/akudo7/kudos-gpt/blob/main/README.md">Settings</a>
  ·
  <a href="https://github.com/akudo7/kudos-gpt/blob/main/README.md">Features</a>
  ·
  <a href="https://github.com/akudo7/kudos-gpt/issues">Support</a>
</h4>


<p align="left">
The kudos-gpt is a ChatGPT-like extension for the VSCode. Now you can have an AI chatbot like the ChatGPT right in the VSCode. Use it as your AI programming assistant which you can talk with to understand complex code, modify and improve your code, or generate comments for your code. The possibilities are endless until the maxTokens actually. To start, turn on it from the command menu, highlight a piece of code, click on the plus icon on the left to open a chat, and start talking with it just like in the ChatGPT. All your conversations are saved and exported in your workspace so you can look back on them automatically when you open files.
</p>

# Usage image
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_preview.png" />
    <font color="red">NOTE: It is confirmed to work on the macOS, Sonoma 14.0 only.</font>
</p>

&nbsp;

# Settings
The kudo-gpt supports many features to ask your requests to AIs with a simple and easy-to-use interface.

<details>
<summary>01. Set the token:</summary>

To enable the kudos-gpt, you need to set the token to the Setting / kudos-gpt / 08 Kudos GPT Toen. You can use the token below because of pre-releasing. To enable setting this value, you have to restart the VSCode again. 

<font color="red">kudo-gpt token for pre-release, it will be working until 2024-03-31.</font>
    
```text
    eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJwcm9kdWN0Ijoia3Vkb3MtZ3B0IiwidmVyc2lvbiI6IjEuMC4wIiwicHVibGlzaCI6InByZS1yZWxlYXNlIiwiaGFzaCI6IjdlZTlkNjZiZGMxYzlmNzQ3NWZjZmRmMWFjZTQ5OTE0ZDNmYzA3MWY1OTFlMmEzZGNkM2U5YmQzMWY4ZmEwMmMiLCJ1c2VySWQiOm51bGwsInRva2VuSWQiOiI5ZmE3MzVlYS02YTFlLTRmMDgtODcwNy0xZGFjYzkyYjViZDIiLCJpYXQiOjE2OTk2MjAyODYsImV4cCI6MTcxMTkyOTYwMH0.Z5Gg1ACzNYAp0dABrfnF0UXFl0f7uissKljImL6O-4R-8wvvaDLpVL8n8TnzYEkgUtIhLu_wfwFW61_LJ3OVzI30NW0q47mSjijRiANp4yLMnqLE8N2bhnuWALpFqswT5QN1k6PQBWDbWJQhkODh0KQYYcbthoaFG5HBKUkLbd8wVBj-MYv45f-BJm5bO49YhqXPoO8u76iQJu5oJovc81Q7wTBWg3WG9z7TDSViZ7egl1f9iAvYa05PZEfRtzcR7wOK-5POUUfATwB5mO1lVCV1KGJthfL2xy0sf-JiXM6DX9xsRTHvo68A_YECBw8fWwiuiNUUkggTF7m3vv8XQA
```

<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_00_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>02. Chose to use the OpenAI or Azure OpenAI:</summary>
&nbsp;
<details>
<summary>OpenAI</summary>

To select the OpenAI, you need to set some values below.
- Setting / kudos-gpt / 01 Service
    - OpenAI
- Setting / kudos-gpt / 02 OpenAI APIKey
    - Your OpenAI APIKey
- Setting / kudos-gpt / 03 Open AI Models
    - gpt-3.5-turbo
    - gpt-3.5-turbo-16k
    - gpt-4
    - gpt-4-32k

To enable setting these values, you have to restart the VSCode again.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_01_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>Azure OpenAI</summary>

To select the Azure OpenAI, you need to set some values below.
- Setting / kudos-gpt / 01 Services
    - Azure OpenAI
- Setting / kudos-gpt / 04 Azure URL
    - Your Azure URL
    - example: `https://kudo-openai-1.openai.azure.com/`
- Setting / kudos-gpt / 05 Azure APIKey
    - Your Azure APIKey
    - example: `12345678901234567l890abcdefghijk`
- Setting / kudos-gpt / 06 Azure Deployment ID
    - Your Azure Deployment ID
    - example: `kudo-35-16k`

To enable setting these values, you have to restart the VSCode again.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_01_2.png" />
</p>
</details>
</details>
&nbsp;
<details>
<summary>03. Adjustment of the AI parameters:</summary>
    
To change the parameters of the OpenAI or Azure OpenAI, you need to edit some values below in settings.json.
- Setting / kudos-gpt / Chat Options
    
```json
"kudos-gpt.chatOptions": {
    "maxTokens": 4000,
    "temperature": 0.7,
    "frequencyPenalty": 0,
    "presencePenalty": 0,
    "topP": 1
},
```

<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_02_1.png" />
</p>
</details>
&nbsp;&nbsp;

<details>
<summary>04. Adjustment of the messages of the buttons:</summary>
    
To change the messages of the buttons, you need to edit some values below in settings.json.

- Setting / kudos-gpt / Messages
```json
"kudos-gpt.messages": {
    "progress": "inquiring...",
    "makeHeader": "The code is as follows",
    "bugAssessment": "Find the bugs in the code, and show the improvements as thimproved code.",
    "vulnerabilityAssessment": "Find and address vulnerabilities in the code, anshow the improvements as the improved code.",
    "speedEnhancement": "Diagnose if code speed improvement is possible, and shothe improvements as the improved code.",
    "etcEnhancement": "Diagnose if any other improvements are possible, and show thimprovements as the improved code.",
    "makeComment": "Add comments for code review to the class, methods, and allines of code as the improved code."
},
```
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_03_1.png" />
</p>
</details>
&nbsp;

# Features
The kudo-gpt supports many features to ask your requests to AIs with a simple and easy-to-use interface.

<details>
<summary>01. Turn On/Off:</summary>

After loading the kudos-gpt successfully, you have to turn it on yourself with the `kudos-gpt: On/Off`.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_1.png" />
</p>
So you can click on the plus icon on the left to create a new chat and also click a note to open a chat.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_2.png" />
</p>
</details>
&nbsp;
<details>
<summary>02. Have a discussion by asking directly:</summary>
To ask your question in a discussion, you can use the `Direct asking` button.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_05_1.png" />
</p>
Your question will be answered from the assistant.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_05_2.png" />
</p>
</details>
&nbsp;
<details>
<summary>03. Have a discussion with templates:</summary>

To start a discussion with the template, you can use strings in the clipboard for the `Clipboard` button.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_06_1.png" />
</p>
To use the Clipboard button, the message will be added as the system.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_06_2.png" />
</p>
To use the buttons, the message will be added as the user.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_06_3.png" />
</p>
After pushing the “Find bugs” for example, a message from the AIs will be from the assistant.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_06_4.png" />
</p>
</details>
&nbsp;
<details>
<summary>04. Save a discussion</summary>

Save discussions are available with the pencil icon `JSON Export`. It will be created a new JSON file as an `opening file + .json`, and also they will be imported automatically when an original file is opened.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_11_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>05. Delete a discussion</summary>

To delete a discussion, you can click the cross icon `del thread`. 
<font color="red">NOTE: It is not removed from a JSON file.</font>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_07_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>06. Delete a message</summary>

To delete a message in a discussion, you can use the `Delete` command from the `More actions…`. 
<font color="red">NOTE: It is not removed from a JSON file.</font>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_08_1.png" />
</p>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_08_2.png" />
</p>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_08_3.png" />
</p>
</details>
&nbsp;
<details>
<summary>07. Edit a message</summary>

To edit a message in a discussion, you can use the `Edit` command from the `More actions…`. To enable the editing, you can use the `save` button. 
<font color="red">NOTE: It is not removed from a JSON file.</font>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_09_1.png" />
</p>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_09_2.png" />
</p>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_09_3.png" />
</p>
</details>
&nbsp;
<details>
<summary>08. Ignore a message in a discussion</summary>

To ignore a message in a discussion, you can use the `Note` command from the `More actions…`.
<font color="red">NOTE: It is not removed from a JSON file.</font>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_10_1.png" />
</p>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_10_2.png" />
</p>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_10_3.png" />
</p>
</details>
&nbsp;
<details>
<summary>09. l10n supporting</summary>

- English
- Japanese

</details>

&nbsp;
# Bonus features(not stable yet)
<details>
<summary>0A. Notion export</summary>

To export a discussion to the Notion, you have to enter a Notion Integration Token beforehand. And then you can click the notion icon `Notion export` and enter a pageId in the dialog. It will be add as a database in the Notion page.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_notion_1.png" />
</p>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_notion_2.png" />
</p>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_notion_3.png" />
</p>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_notion_4.jpg" />
</p>
</details>

## Enjoy coding, and have fun!

## **Hand-crafted by [Akira Kudo](https://www.linkedin.com/in/akira-kudo-4b04163/) in Tokyo, Japan**

<p align="center">Copyright and Reversed &copy; 2023-present Akira Kudo</p>
