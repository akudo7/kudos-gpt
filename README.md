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
&nbsp;

# New features

- <font color="red" size=5>ver 2.1.0</font>
  - Supported the RAG with the OpenAI.
  - Fixed not saving multiple threads.
  - Fixed making same comments when open a file before saving its json.
        <p align="center">
        <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v2.1.0.gif" />
        </p>
- <font size=5>ver 2.0.0</font>
  - Supporting the new Assistants API with the OpenAI, event it's still "BETA".
        <p align="center">
        <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v2.0.0.gif" />
        </p>
- <font size=5>ver 1.1.1</font>
  - Changed the button "Clipboard" to "System", and no longer need to put any strings to the Clipboard    before pushing it.
  - Added the feature "Compare" that is available to compare/edit an active text editor with a comment.
  - Added the button "Terminal" that is available to create a chat from outputs from a terminal.
  - Fixed the button "Terminal" is also pasting outputs to a terminal.
        <p align="center">
        <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v1.1.0.gif" />
        </p>

&nbsp;

# Settings

The kudo-gpt supports many features to ask your requests to AIs with a simple and easy-to-use interface.

<details>
<summary><font color="red" size=5>ver 2.1.0</font></summary>
<details>
 <summary>01. Set the token:</summary>
</br>
To enable the kudos-gpt, the token below needs to be set to the Setting / kudos-gpt / 08 Kudos GPT Toen. To enable setting this value, the VSCode has to be restarted.
</br>
</br>
<font color="red">kudo-gpt token for pre-release, it will be working until 2024-03-31.</font>

```text
eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJwcm9kdWN0Ijoia3Vkb3MtZ3B0IiwidmVyc2lvbiI6IjIuMS4wIiwicHVibGlzaCI6InByZS1yZWxlYXNlIiwiaGFzaCI6IjE0NDEzZDk5ZDgxODcxMmFjZjdlMDFlNTdkN2ViNDY4YTllZmM0Zjg4NGRiNTZkMmM1NDNjY2VkYjI5ZmRlMzQiLCJ1c2VySWQiOm51bGwsInRva2VuSWQiOiJiM2Q1NTA3MS0wYWU3LTQ5ODYtYTA3YS0wMmM5NWYzNDdmMWYiLCJpYXQiOjE3MDI4OTAxMjksImV4cCI6MTcxMTkyOTYwMH0.owpYgYBxgrgfXCn86McZfeDvkaGqCoGA1cKQJ0NwNw0ifURLT5XLxccJYvb_vqcPV4-d1UHWDMcOUg_3OpuucU6GTfSKEBds9Lg0WrznAe8KUjJsdtiMI4buYXVFBkG5Aare_ipAmtjm0u5LsJPjjcwZ4cCu4Gv7rBTeQmxkZEm9zY27bPBYlfQZYRjBNPLZCAO3ewUp-rDOm3gYpS9nipWiwWtXt2p8lgz1bsi7AaWSyIuBQnvkuwJzGtFhD5MHSJbMhxVguFjxBCBuiKeSavu-k8EecfS5r-uVVKz5nOgtlJHeYWWfKpsQVD2pTKv4_0uqMITNzrSZfP4L446hrQ
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
  - <font color="red">gpt-4-1106-preview</font>

To enable these values, the VSCode has to be restarted.
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

To enable these values, the VSCode has to be restarted.
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
    `</p>
</details>
&nbsp;&nbsp;

<details>
<summary>04. Adjustment of the messages of the buttons:</summary>

To change the messages of the buttons, some values below have to be edited in settings.json.

- <font color="red">Setting / kudos-gpt / Messages</font>

    ```json
    "kudos-gpt.messages": {
        "progress": "inquiring...",
        "autoSystem": "The code is as follows",
        "manualSystem": "The code is as follows",
        "bugAssessment": "Find the bugs in the code, and show the improvements as the improved code.",
        "vulnerabilityAssessment": "Find and address vulnerabilities in the code, and show the improvements as the improved code.",
        "speedEnhancement": "Diagnose if code speed improvement is possible, and show the improvements as the improved code.",
        "etcEnhancement": "Diagnose if any other improvements are possible, and show the improvements as the improved code.",
        "makeComment": "Add comments for code review to the class, methods, and all lines of code as the improved code.",
        "terminal": "Here are the results. Let me know if any corrections are needed and provide suggestions for improvement."
    },
    ```

    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_03_1.png" />
    </p>
</details>
&nbsp;

<details>
<summary>05. Adjustment of the temporary folder:</summary>

To change the temporary folder, a value below have to be edited in settings.json.

- Setting / kudos-gpt / Temp Folder

    ```json
    /var/tmp
    ```

    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_30_0.png" />
    </p>
</details>
</details>
&nbsp;

<details>
<summary><font size=5>ver 2.0.0</font></summary>
<details>
 <summary>01. Set the token:</summary>
</br>
To enable the kudos-gpt, the token below need to be set to the Setting / kudos-gpt / 08 Kudos GPT Toen. To enable setting this value, the VSCode have to be restarted.
</br>
</br>
<font color="red">kudo-gpt token for pre-release, it will be working until 2024-03-31.</font>

```text
eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJwcm9kdWN0Ijoia3Vkb3MtZ3B0IiwidmVyc2lvbiI6IjIuMC4wIiwicHVibGlzaCI6InByZS1yZWxlYXNlIiwiaGFzaCI6IjJlMmFkOWQwZmFiOWI2Zjc1NzNmMzMyZDcwM2Q3YTdhNDgxZWRiNGM5NDMzYWE4ZjM3ZjA2YWRiYmMxMTE5NjEiLCJ1c2VySWQiOm51bGwsInRva2VuSWQiOiIwZDAwYmNiNC0xZjQ3LTRmNTUtYTExYy0xMmRkY2EwN2EwMjQiLCJpYXQiOjE3MDIwNDMyNjAsImV4cCI6MTcxMTkyOTYwMH0.p880eZzceNHSU0eolov-8Ddjhsa7Ez5UP3ODEOTMOqM6yLGNtA-_gmgGB7JmR7pXdPJ1_tARzEL7N3Zc0Y0xPgDuRoe7KiekX73xEDFfuxooW3cR9A36dwmgfVRfml9hihGGeUiHwIQVCh9mZVAaCQSrKKL9GSNGcNPGHM2KSJXVZjK04vty7JyqKuotYwtYDuQCn-hgjMqPrBmTzho0IUyHSbnLd8S4iaXAnwRb5I_sfvNMKCVgc88PQYM-PRT3avyzbwoHq-6EMpfYesQbpLuEGcL9VxLaeqyqiCQXab28ojq2-5XXay5R45rxT_a3tN_ES-YN3iuthPdE7c64zQ
```

<p align="center">
<img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_00_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>02. Choose the OpenAI or Azure OpenAI: <font color="red">New feature is available.</font></summary>
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
  - <font color="red">gpt-4-1106-preview</font>

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
    `</p>
</details>
&nbsp;&nbsp;

<details>
<summary>04. Adjustment of the messages of the buttons:<font color="red">New feature is available.</font></summary>

To change the messages of the buttons, some values below have to be edited in settings.json.

- <font color="red">Setting / kudos-gpt / Messages</font>

    ```json
    "kudos-gpt.messages": {
        "progress": "inquiring...",
        "autoSystem": "The code is as follows",
        "manualSystem": "The code is as follows",
        "bugAssessment": "Find the bugs in the code, and show the improvements as the improved code.",
        "vulnerabilityAssessment": "Find and address vulnerabilities in the code, and show the improvements as the improved code.",
        "speedEnhancement": "Diagnose if code speed improvement is possible, and show the improvements as the improved code.",
        "etcEnhancement": "Diagnose if any other improvements are possible, and show the improvements as the improved code.",
        "makeComment": "Add comments for code review to the class, methods, and all lines of code as the improved code.",
        "terminal": "Here are the results. Let me know if any corrections are needed and provide suggestions for improvement."
    },
    ```

    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_03_1.png" />
    </p>
</details>
&nbsp;

<details>
<summary>05. Adjustment of the temporary folder:</summary>

To change the temporary folder, a value below have to be edited in settings.json.

- Setting / kudos-gpt / Temp Folder

    ```json
    /var/tmp
    ```

    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_30_0.png" />
    </p>
</details>
</details>
&nbsp;

<details>
<summary><font size=5>ver 1.1.1</font></summary>
<details>
<summary>01. Set the token:</summary>
</br>
To enable the kudos-gpt, the token below need to be set to the Setting / kudos-gpt / 08 Kudos GPT Toen. To enable setting this value, the VSCode have to be restarted.
</br>
</br>
 <font color="red">kudo-gpt token for pre-release, it will be working until 2024-03-31.</font>

```text
    eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJwcm9kdWN0Ijoia3Vkb3MtZ3B0IiwidmVyc2lvbiI6IjEuMS4xIiwicHVibGlzaCI6InByZS1yZWxlYXNlIiwiaGFzaCI6ImQzOGIzY2NjMzU3OGZjYzE4ZjZiOGVmMTdmY2U1MTc0NDVmZWRjN2Q5NjQ0MjI2YzI4ZWY0MWU3MzYwM2ViZDMiLCJ1c2VySWQiOm51bGwsInRva2VuSWQiOiIyMGE4MzM1Ni02M2EwLTRmMDItYThmMS1lZWZlNDU0ZTZkYzkiLCJpYXQiOjE3MDE0MjAxNTgsImV4cCI6MTcxMTkyOTYwMH0.FJaLU8IuiczWk7m7Tar4ZT-IvPsTmqNKUBINZWMedgrqgr2aLYYkSIUF7YOX2Z_6_5URQLeEPq-N8NiEFTqnhx4VQ4Pr1dnSBDZVFRQ2UF44RIUq_STCguy8kAX4x6kEK__i83ZbM_avRVvS9StkQFcoMGbS2fi1u6FbGOs_pNPWUl5c5jRe8dx0rVMTSVbbLSCkIxb-2zyRZU-LmQ3WVak5NBfCJA7WvvWpjg5k4hX1S6c6ym52n-6pyWtndMBg0b6lkEWr9mfRsX5XlQvqei3vyCrgH1Ag63mwbTqABGeYDpcfXlChShpx7vZMn96wWb-dz_bTCZA2-asBXlEdrw
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
<summary>04. Adjustment of the messages of the buttons:</summary>

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
<summary>05. Adjustment of the temporary folder:</summary>

To change the temporary folder, a value below have to be edited in settings.json.

- Setting / kudos-gpt / Temp Folder

```json
/var/tmp
```

<p align="center">
<img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_30_0.png" />
</p>
    </details>
</details>
&nbsp;









# Features

The kudo-gpt supports many features to ask your requests to AIs with a simple and easy-to-use interface.

<details>
<summary><font color="red" size=5>ver 2.1.0</font></summary>
<details>
<summary>01. Turn On/Off:</summary>

After loading the kudos-gpt successfully, the `kudos-gpt: On/Off` has to be executed yourself for turnning it on.
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
<summary>02. Start a discussion with the system:</summary>

The button "Auto System" and "Manual Systerm" are available to create aa system for a new discussion.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_v2_20_0.png" />
</p>
The button "Auto System" doesn't need to put any strings to the clipboard before pushing the button. All strings from an active text editor will be added to a message with the "kudos-gpt.messages.autoSystem" prompt in the settings.
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
To use the Clipboard button, a message will be added as the system.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_06_2.png" />
</p>
To use the buttons, a message will be added as the user.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_06_3.png" />
</p>
After pushing the “Find bugs” for example, a message from the AIs will be added as the system.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_06_4.png" />
</p>
</details>
&nbsp;
<details>
<summary>05. Create a message from a terminal:</summary>

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

To Save a log in a discussion is available with the pencil icon `JSON Export`. It will be created a new JSON file as an `opening file + .json` for the Azure OpenAI, <font color="red">and also `opening file + .{model name}.openai.json` that has a threadId and assistantId for the OpenAI.</font> They will be imported automatically when an original closed file is opened.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_11_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>07. Delete a discussion: <font color="red">New feature is available.</font></summary></summary>

To delete a discussion, the cross icon `del thread` is available.
<font color="red">NOTE: It is removed from a JSON file, and also deleting the thread, assistant and RAG files from the OpenAI.</font>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_07_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>08. Add a file to the discussion: <font color="red">New feature is available.</font></summary>

To add a file to a discussion for the RAG feature, the icon `Add a file to the assistant`is available. And the "RAG" exploerer will be appeared for deleting and reloading it from the discussions after that.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_50_1.png" />
</p>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_50_2.png" />
</p>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_50_3.png" />
</p>
</details>
&nbsp;
<details>
<summary>09. Delete a message</summary>

To delete a message in a discussion, the `Delete` command from the `More actions…` is available. This feature works for the Azure OpenAI.
<font color="red">NOTE: It is not removed from a JSON file automatically.</font>
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
<summary>10. Edit a message</summary>

To edit a message in a discussion, the `Edit` command from the `More actions…` is available. And the `save` button is available for enabling the editing. This feature works for the Azure OpenAI.
<font color="red">NOTE: It is not removed from a JSON file automatically.</font>
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
<summary>11. Ignore a message in a discussion</summary>

To ignore a message in a discussion, the `Note` command from the `More actions…` is available. This feature works for the Azure OpenAI.
<font color="red">NOTE: It is not removed from a JSON file automatically.</font>
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
<summary>12. Compare/update an active text editor with a message</summary>

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
<summary>13. l10n supporting</summary>

- English
- Japanese

</details>
</details>
&nbsp;

<details>
<summary><font size=5>ver 2.0.0</font></summary>
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

The button "Auto System" and "Manual Systerm" are available to create aa system for a new discussion.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_v2_20_0.png" />
</p>
The button "Auto System" doesn't need to put any strings to the clipboard before pushing the button. All strings from an active text editor will be added to a message with the "kudos-gpt.messages.autoSystem" prompt in the settings.
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
<summary>05. Create a message from a terminal:</summary>

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
<summary>06. Save a discussion<font color="red"> New feature is available.</font></summary>

Save discussions are available with the pencil icon `JSON Export`. It will be created a new JSON file as an `opening file + .json` for the Azure OpenAI, <font color="red">and also `opening file + .{model name}.openai.json` that has a threadId and assistantId for the OpenAI.</font> They will be imported automatically when an original file is opened.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_11_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>07. Delete a discussion<font color="red"> New feature is available.</font></summary></summary>

To delete a discussion, the cross icon `del thread` is available.
<font color="red">NOTE: It is not removed from a JSON file, but it tries deleting the thread and assistant from the OpenAI.</font>
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
<summary>11. Compare/update an active text editor with a message</summary>

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
</details>
&nbsp;

<details>
<summary><font size=5>ver 1.1.1</font></summary>
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
<summary>02. Start a discussion with the system:</summary>

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
<summary>05. Create a message from a terminal:</summary>

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
<summary>11. Compare/update an active text editor with a message</summary>

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

- Replacing the Assistants API with the Azure OpenAI
- Supporting the retrieval with the Azure OpenAI
- Local LLMs

## **Hand-crafted by [Akira Kudo](https://www.linkedin.com/in/akira-kudo-4b04163/) in Tokyo, Japan**

<p align="center">Copyright and Reversed &copy; 2023-present Akira Kudo</p>
