<h1 align="center">kudos-gpt</h1>

<h4 align="center">
  <a href="https://github.com/akudo7/kudos-gpt/blob/main/README.md#settings">Settings</a>
  ·
  <a href="https://github.com/akudo7/kudos-gpt/blob/main/README.md#features">Features</a>
  ·
  <a href="https://github.com/akudo7/kudos-gpt/issues">Support</a>
</h4>



<p align="left">
The kudos-gpt is a ChatGPT-like extension for the VSCode. Now you can have an AI chatbot like the ChatGPT right in the VSCode. Use it as your AI programming assistant which you can talk with to understand complex code, modify and improve your code, or generate comments for your code. The possibilities are endless until the maxTokens actually. To start, turn on it from the command menu, highlight a piece of code, click on the plus icon on the left to open a chat, and start talking with it just like in the ChatGPT. All your conversations are saved and exported in your workspace so you can look back on them automatically when you open files.
</p>

# Usage image
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v1.1.0.gif" />
    <font color="red">NOTE: It is confirmed to work on the macOS, Sonoma 14.0 only.</font>
</p>

&nbsp;

# Settings
The kudo-gpt supports many features to ask your requests to AIs with a simple and easy-to-use interface.

<details>
<summary>01. Set the token:<font color="red"> New token for v1.1.0 is available.</font></summary>

To enable the kudos-gpt, the token below need to be set to the Setting / kudos-gpt / 08 Kudos GPT Toen. To enable setting this value, the VSCode have to be restarted.

<font color="red">kudo-gpt token for pre-release, it will be working until 2024-03-31.</font>
    
```text
    eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJwcm9kdWN0Ijoia3Vkb3MtZ3B0IiwidmVyc2lvbiI6IjEuMS4wIiwicHVibGlzaCI6InByZS1yZWxlYXNlIiwiaGFzaCI6Ijg1NDBmYjQ5NGZhNDMyOGYxZGU4YzdkY2Q5Mzk2ZjY1NDZiYTdkMjg0ZGVlNWM1MWI0ZGI1YjA0YjhmMWE1YTkiLCJ1c2VySWQiOm51bGwsInRva2VuSWQiOiI1ODU0NTI2YS0xYWM0LTRhYTItODA3OC1jNjcyOTJkN2U3MmQiLCJpYXQiOjE3MDA5MTcyMjgsImV4cCI6MTcxMTkyOTYwMH0.eAO3lD1U01aiv6Nc-PbeKSz0qMP8mnbHgSHRYLiuyLmnfOg_LIZW0OQJyz-SsMITPzDyDJRkxp3C0drJBXOTny4OGwjKTN2dJauz4F4x9B03_29JOATPnToVK2t6_LpiOiuMcAGIvMqQrTRya8Kzh1hHe36gA4yV8biG5XxhNwwBmReGSk74cTPY-jXDEK0kEH7XZbe-iQyactQu9j-PuNvrrmEMSEFUyZO9EPzW_i5JbPkt3hQ8tQkiaNQVj3HthjqZ1ACxrU1WDzMIrwXisWm4MShGK1xCvTaAC4PE2mKXCXOeEUDTaJ464cbVixRM_BsthP6zL3qLper2PULWEQ
```

<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_00_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>02. Choose the OpenAI or Azure OpenAI:</summary>
&nbsp;
<details>
<summary>OpenAI</summary>

To use the OpenAI, some values below have to be set.
- Setting / kudos-gpt / 01 Service
    - OpenAI
- Setting / kudos-gpt / 02 OpenAI APIKey
    - Your OpenAI APIKey
- Setting / kudos-gpt / 03 Open AI Models
    - gpt-3.5-turbo
    - gpt-3.5-turbo-16k
    - gpt-4
    - gpt-4-32k

To enable these values, the VSCode have to be restarted.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_01_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>Azure OpenAI</summary>

To use the Azure OpenAI, some values below have to be set.
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

To enable these values, the VSCode have to be restarted.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_01_2.png" />
</p>
</details>
</details>
&nbsp;
<details>
<summary>03. Adjustment of the AI parameters:</summary>
    
To change the parameters of the OpenAI and Azure OpenAI, some values below have to be edited in settings.json.
- Setting / kudos-gpt / Chat Options
    
```json
"kudos-gpt.chatOptions": {
    "maxTokens": 4000,
    "temperature": 0.3,
    "frequencyPenalty": 0,
    "presencePenalty": 0,
    "topP": 0.2
},
```

<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_02_1.png" />
</p>
</details>
&nbsp;&nbsp;

<details>
<summary>04. Adjustment of the messages of the buttons: <font color="red"> New feature is available.</font></summary>
    
To change the messages of the buttons, some values below have to be edited in settings.json.

- Setting / kudos-gpt / Messages
```json
"kudos-gpt.messages": {
    "progress": "inquiring...",
    "makeHeader": "The code is as follows",
    "bugAssessment": "Find the bugs in the code, and show the improvements as thimproved code.",
    "vulnerabilityAssessment": "Find and address vulnerabilities in the code, anshow the improvements as the improved code.",
    "speedEnhancement": "Diagnose if code speed improvement is possible, and shothe improvements as the improved code.",
    "etcEnhancement": "Diagnose if any other improvements are possible, and show thimprovements as the improved code.",
    "makeComment": "Add comments for code review to the class, methods, and allines of code as the improved code.",
    "terminal": "Here are the results. Let me know if any corrections are needed and provide suggestions for improvement."
},
```
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_03_1.png" />
</p>
</details>
&nbsp;

<details>
<summary>05. Adjustment of the temporary folder: <font color="red"> New feature is available.</font></summary>
    
To change the temporary folder, a value below have to be edited in settings.json.

- Setting / kudos-gpt / Temp Folder
```json
/var/tmp
```
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_30_0.png" />
</p>
</details>
&nbsp;

# Features
The kudo-gpt supports many features to ask your requests to AIs with a simple and easy-to-use interface.

<details>
<summary>01. Turn On/Off:</summary>

After loading the kudos-gpt successfully, the `kudos-gpt: On/Off` have to be executed yourself for turnning it on.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_1.png" />
</p>
So the plus icon on the left will be available for creating/opening a discussion.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_2.png" />
</p>
</details>
&nbsp;
<details>
<summary>02. Start a discussion with the system: <font color="red"> New feature is available.</font></summary>

The button "System" is available to create a discussion from the system. 
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_20_0.png" />
</p>
No longer need to put any strings to the clipboard before pushing the button. All strings from an active text editor will be added to a message with a "kudos-gpt.messages.makeHeader" prompt in the settings.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_20_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>03. Have a discussion by asking directly:</summary>
To ask your question in a discussion, the `Direct asking` button is available.
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
<summary>04. Have a discussion with templates:</summary>

To start a discussion with the template, strings in the clipboard are available with the `Clipboard` button.
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
After pushing the “Find bugs” for example, a message from the AIs will be added as the assistant.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_06_4.png" />
</p>
</details>
&nbsp;
<details>
<summary>05. Create a message from a terminal:<font color="red"> New feature is available.</font></summary>

To create a message with the output from a terminal is available with the `Terminal` button. All strings from a terminal will be added to a message with a "kudos-gpt.messages.terminal" prompt in the settings.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_21_0.png" />
</p>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_21_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>06. Save a discussion</summary>

Save discussions are available with the pencil icon `JSON Export`. It will be created a new JSON file as an `opening file + .json`, and also they will be imported automatically when an original file is opened.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_11_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>07. Delete a discussion</summary>

To delete a discussion, the cross icon `del thread` is available. 
<font color="red">NOTE: It is not removed from a JSON file.</font>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_07_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>08. Delete a message</summary>

To delete a message in a discussion, the `Delete` command from the `More actions…` is available.
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
<summary>09. Edit a message</summary>

To edit a message in a discussion, the `Edit` command from the `More actions…` is available. And the `save` button is available for enabling the editing.
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
<summary>10. Ignore a message in a discussion</summary>

To ignore a message in a discussion, the `Note` command from the `More actions…` is available.
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
<summary>11. Compare/update an active text editor with a message<font color="red"> New feature is available.</font></summary>

To compare/update an active text editor with a message in a discussion, the `Compare` command from the `More actions…` is available.
<font color="red">NOTE: A temporary file will be created in a folder `Setting / kudos-gpt / Temp Folder`.</font>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_40_0.png" />
</p>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_40_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>12. l10n supporting</summary>

- English
- Japanese

</details>

&nbsp;
# Bonus features(not stable yet)
<details>
<summary>0A. Notion export</summary>
To export a discussion to the Notion, a Notion Integration Token have to be entered beforehand. And then the notion icon `Notion export` will be available and will be able to enter a pageId in the dialog. It will be add as a database in the Notion page.
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

&nbsp;
# Comming features soon(I hope...)
- RAG
- Replace the Assistants API as new one
- Local LLMs

## **Hand-crafted by [Akira Kudo](https://www.linkedin.com/in/akira-kudo-4b04163/) in Tokyo, Japan**

<p align="center">Copyright and Reversed &copy; 2023-present Akira Kudo</p>
