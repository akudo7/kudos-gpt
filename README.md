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

<font color="red" size=5>ver 5.0.1</font>

- Unlock expire day
  - No longer need to set the KudosGpt Token
- Fixed to redraw problem on the Configuration Tab.

The next major version will no longer work with Flowise due to the use of a new DAG engine, which calls LangChain directly. As a result, some features that work with Flowise will be deprecated.
This is why this version does not require setting the KudosGpt token. I look forward to you upgrading to the next major version "kudosflow".

  <p align="center">
  <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudosflow.png"/>
  </p>

- <font size=5>ver 5.0.0</font>
  <details> 
  - Supported Devin feature
    - Available to import XMLs which are exported by the Bolt.new system promopt.
      - See in detail of the original prompt at the "https://github.com/stackblitz/bolt.new/blob/main/app/lib/.server/llm/prompts.ts".
        - Recommend to change it for fitting with your environment.
      - boltArtifact and bolt_file_modifications are supported.
      - Samples
        - [System Prompt](https://github.com/akudo7/kudos-gpt/raw/HEAD/bolt_new-system-prompt.txt) 
        - [artifact.xml](https://github.com/akudo7/kudos-gpt/raw/HEAD/artifact.xml) 
        - [modifications.xml](https://github.com/akudo7/kudos-gpt/raw/HEAD/modifications.xml) 
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v5.0.0_1.gif"/>
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v5.0.0_2.gif"/>
    </p>
  </details>
- <font size=5>ver 4.6.0</font>
  <details>
  - Supported the Flowise-SDK
    - Available to receive stream responses from LLM.
    - No longer need to set api version in the Flowise URL on the Assistant tab.
      - it must be set as 'http://localhost:3000' from 'http://localhost:3000/apiv1'.
  <p align="center">
  <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.6.0.gif"/>
  </p>
  </details>
- <font size=5>ver 4.5.0</font>
  <details>
  - Supporting the Flowise API Key
    - Need to set a Flowise API Key on the Assistant tab.
    - Flowise API needs it from v2.0.6.
  <p align="center">
  <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.5.0_1.png"/>
  </p>
  </details>
- <font size=5>ver 4.4.0</font>
  <details>
  - The new button "Asking image" is available to ask questions with an image.
    - Input a question is required before push it.
  - No need to change a FlowiseChatId on the configuration window for change the conversation.
    - The name of answer is used as FlowiseChatName.
  <p align="center">
  <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.4.0_1.gif"/>
  </p>
  </details>
- <font size=5>ver 4.3.0</font>
  <details>
  - Available to inject a chat with a chatId and keep to continue the conversation.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.3.0_1.gif"/>
    </p>
  </details>
- <font size=5>ver 4.2.0</font>
  <details>
  - Available to show the File links when the "Return Source documents" of Flowise chain node is enabled.
  - The timeout of fetch function is set as 15mins.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.2.0_1.png"/>
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.2.0_2.png"/>
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.2.0_3.png"/>
    </p>
  </details>
- <font size=5>ver 4.1.0</font>
  <details>
  - New configuration window
  - Setting the kudo-gpt token is only available on the user settings now.
  - No longer need to re-open the VSCode after values on it are changed.
    - Available to select a FlowiseChartId as a pulldown menu from the Flowise directly.
        <p align="center">
        <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_1.png"/>
        <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png"/>
        <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_3.png"/>
        <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_4.png"/>
        </p>
  </details>
- <font size=5>ver 4.0.0</font>
  <details>
    - Focusing the Assistant to use LLMs, RAG, Agents and etc via the [Flowise](https://github.com/FlowiseAI/Flowise?tab=readme-ov-file).
      - <font color="red">Recommend to confirm working it beforehands</font>.
          <p align="center">
          <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.0.0_1.png"/>
          <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.0.0_2.png"/>
          <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.0.0_3.png"/>
          </p>
  </details>
- <font size=5>ver 3.0.0</font>
  <details>
    - Supported the Copilot feature like the Github Copilot.
    - Supported the Ollama to the Assistant.
      - <font color="red">Recommend to confirm working it with a UI like [ollama-webui](https://github.com/ollama-webui/ollama-webui) beforehands.</font>
          <p align="center">
          <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v3.0.0_1.gif" />
          <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v3.0.0_2.jpeg" />
          <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v3.0.0_3.jpeg" />
          </p>
  </details>
- <font size=5>ver 2.2.0</font>
  <details>
    - Supported the GPT4ALL.
      - <font >Recommend to confirm working it with the GPT4ALL <a href="https://github.com/nomic-ai/gpt4all?tab=readme-ov-file#chat-client">Chat Client</a> beforehands.</font>.
    - Fixed an error with deleting a thread before saving.
        <p align="center">
        <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v2.2.0_1.png" />
        <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v2.2.0_2.png" />
        </p>
  </details>
- <font size=5>ver 2.1.0</font>
  <details>
    - Supported the RAG with the OpenAI.
    - Fixed not saving multiple threads.
    - Fixed making same comments when open a file before saving its json.
        <p align="center">
        <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v2.1.0.gif" />
        </p>
  </details>
- <font size=5>ver 2.0.0</font>
  <details>
    - Supporting the new Assistants API with the OpenAI, event it's still "BETA".
        <p align="center">
        <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v2.0.0.gif" />
        </p>
  </details>
- <font size=5>ver 1.1.1</font>
  <details>
    - Changed the button "Clipboard" to "System", and no longer need to put any strings to the Clipboard before pushing it.
    - Added the feature "Compare" that is available to compare/edit an active text editor with a comment.
    - Added the button "Terminal" that is available to create a chat from outputs from a terminal.
    - Fixed the button "Terminal" is also pasting outputs to a terminal.
        <p align="center">
        <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v1.1.0.gif" />
        </p>
  </details>

&nbsp;

# Settings

The kudo-gpt supports many features to ask your requests to AIs with a simple and easy-to-use interface.

<summary><font color="red" size=5>ver 5.0.0</font></summary>
&nbsp;
<details>
 <summary>01. Set the token: <font color="red">New feature is available.</font></summary>
</br>
To enable the kudos-gpt, the token below needs to be set to the Setting / kudos-gpt / 08 Kudos GPT Toen. To enable setting this value, the VSCode has to be restarted.
</br>
</br>
<font color="red">kudo-gpt token for pre-release, it will be working until 2025-03-31.</font>

```text
eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJwcm9kdWN0Ijoia3Vkb3MtZ3B0IiwidmVyc2lvbiI6IjUuMC4wIiwicHVibGlzaCI6InByZS1yZWxlYXNlIiwiaGFzaCI6IjE4ZTg1ZjZiN2I2OTU1YzM5NWMwMTU2NzZlZjM2MTg2OTJlY2FhZmZlNDI4NTlmNWMzOGJkYWYwZWUzMTI3YjUiLCJ1c2VySWQiOm51bGwsInRva2VuSWQiOiJiYzUwODk5NC1mN2MwLTQ3MGItOTYxMS00NzVlZTE4OTE2ZTYiLCJpYXQiOjE3MzU2NTAzMzIsImV4cCI6MTc0MzM3OTIwMH0.rNCv_J2QqvgzB92QU2scVqIsIKSUAjOYkiWjOpbQuMV4Wfoa1u57-8G5em5h9XN1mOJiIIc7TaHXpmHDav72jNPQlaRd9-SF9EXwzrFP16Ge9pmOZAlLx-YaneT_F_08-fWsf0bfeCqDpQcltUQdzxLNDxGnh5nI-BhHfg34OwhoieNHq3k13UUH20XYZU03YdKU1QH32ZQKxUd7clFztslWq-gFUQqdHP1lYDT4wTi1nlhVuhfBX9q_I3tTop5iieS1cmmX3S9MYd3fkAjE9X9YK9_co0lAL2uPRZ1Q0flznTqHcyVCQlL6UjbdYcJX9gUz_mjdRrTe1Tx3b_26yQ
```
<p align="center">
<img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_00_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>02. Set for the Assistant: New feature is available.</summary>
&nbsp;

The command "kudos-gpt: show configuration" is available to set values below for the Assistant.

- Flowise API Key
  - example: `FK9DVbyGQYRcs9uv9RqCGVuGpxqcL+pcXj/XhA494o4=`
- Flowise URL
  - example: `http://localhost:3000`
- Flowise ChatFlow ID
  - example: `00000000-0000-0000-0000-000000000000`
- Temp Folder
  - example: `/var/tmp`
- Messages
  - clipboard
    - example: `The code:`
  - progress
    - example: `inquiring...`
  - bugAssessment
    - example: `Find the bugs in the code, and show the improvements as the improved code.`
  - vulnerabilityAssessment
    - example: `Find and address vulnerabilities in the code, and show the improvements as the improved code.`
  - speedEnhancement
    - example: `Diagnose if code speed improvement is possible, and show the improvements as the improved code.`
  - etcEnhancement
    - example: `Diagnose if any other improvements are possible, and show the improvements as the improved code.`
  - makeComment
    - example: `Add comments for code review to the class, methods, and all lines of code as the improved code.`
  - makeTest
    - example: `Make tests for the code.`
  - terminal
    - example: `Here are the results. Let me know if any corrections are needed and provide suggestions for improvement.`
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png"/>
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_3.png"/>
</p>
</details>
&nbsp;

<details>
<summary>03. Set for the Copilot:</summary>
The command "kudos-gpt: show configuration" is available to set values below for the Copilot.

- Services
  - example: `Ollama`
- Host
  - example: `http://127.0.0.1:11434`
- Model
  - example: `deepseek-coder:1.3b-base-q4_1`
- FIM
  - example: `starcoder`
- num_predict
  - example: `10`
- temperature
  - example: `0.1`

<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png"/>
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_4.png"/>
</p>
</details>
&nbsp;


<details>
<summary><font size=5>ver 4.6.0</font></summary>
&nbsp;
<details>
 <summary>01. Set the token: <font color="red">New feature is available.</font></summary>
</br>
To enable the kudos-gpt, the token below needs to be set to the Setting / kudos-gpt / 08 Kudos GPT Toen. To enable setting this value, the VSCode has to be restarted.
</br>
</br>
<font color="red">kudo-gpt token for pre-release, it will be working until 2025-03-31.</font>

```text
eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJwcm9kdWN0Ijoia3Vkb3MtZ3B0IiwidmVyc2lvbiI6IjQuNi4wIiwicHVibGlzaCI6InByZS1yZWxlYXNlIiwiaGFzaCI6IjliNzQ1ODhkMzU2NWUzMDlhMmUyZjEzZjhiNGI1YzM2MmQ5NjZiMTEwNTVkNGM0MGE4N2I0OTQ4MDI4MjExNTAiLCJ1c2VySWQiOm51bGwsInRva2VuSWQiOiJhZTQ0NWE5Mi0wYzNkLTQ4NTItYjQ3ZS05Mjc1NzUyN2YwMTciLCJpYXQiOjE3MjcxODc2NDMsImV4cCI6MTc0MzM3OTIwMH0.rqGjZdKIaRmay_TMOCZ24WEaqMJhePDODJEU22fM7pjFofczG8GikQje_y79SkNqKIjO91yBbFqUOORkarRqheZ6uEvcIcWNsO6e-k4KAHXvPIaQ3DkIDRBrxS3Spab1V3qMZaoDGW1ThQWPCmO_rRoh0Wi5L6yvTCmK_w2Dp36LAwJ0hME2hScnmopmW4I_TiymjjonlxsKy1czmO6AYzNAyALHkUT7A82WVst8MOgw9wnMZZUfOQrmkX18awchJh0KA4L15jkZCxA0SBRpmXxMKclP4lbViPT31gjQwxMfY8_NSPbotNPpxQydY-NrrxhHdnjJl8anfLczrEn7tg
```
<p align="center">
<img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_00_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>02. Set for the Assistant: <font color="red">New feature is available.</font></summary>
&nbsp;

The command "kudos-gpt: show configuration" is available to set values below for the Assistant.

- Flowise API Key
  - example: `FK9DVbyGQYRcs9uv9RqCGVuGpxqcL+pcXj/XhA494o4=`
- Flowise URL
  - example: `http://localhost:3000`
- Flowise ChatFlow ID
  - example: `00000000-0000-0000-0000-000000000000`
- Temp Folder
  - example: `/var/tmp`
- Messages
  - clipboard
    - example: `The code:`
  - progress
    - example: `inquiring...`
  - bugAssessment
    - example: `Find the bugs in the code, and show the improvements as the improved code.`
  - vulnerabilityAssessment
    - example: `Find and address vulnerabilities in the code, and show the improvements as the improved code.`
  - speedEnhancement
    - example: `Diagnose if code speed improvement is possible, and show the improvements as the improved code.`
  - etcEnhancement
    - example: `Diagnose if any other improvements are possible, and show the improvements as the improved code.`
  - makeComment
    - example: `Add comments for code review to the class, methods, and all lines of code as the improved code.`
  - makeTest
    - example: `Make tests for the code.`
  - terminal
    - example: `Here are the results. Let me know if any corrections are needed and provide suggestions for improvement.`
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png"/>
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_3.png"/>
</p>
</details>
&nbsp;

<details>
<summary>03. Set for the Copilot:</summary>
The command "kudos-gpt: show configuration" is available to set values below for the Copilot.

- Services
  - example: `Ollama`
- Host
  - example: `http://127.0.0.1:11434`
- Model
  - example: `deepseek-coder:1.3b-base-q4_1`
- FIM
  - example: `starcoder`
- num_predict
  - example: `10`
- temperature
  - example: `0.1`

<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png"/>
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_4.png"/>
</p>
</details>
</details>
&nbsp;



<details>
<summary><font size=5>ver 4.5.0</font></summary>
&nbsp;
<details>
 <summary>01. Set the token: <font color="red">New feature is available.</font></summary>
</br>
To enable the kudos-gpt, the token below needs to be set to the Setting / kudos-gpt / 08 Kudos GPT Toen. To enable setting this value, the VSCode has to be restarted.
</br>
</br>
<font color="red">kudo-gpt token for pre-release, it will be working until 2025-03-31.</font>

```text
eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJwcm9kdWN0Ijoia3Vkb3MtZ3B0IiwidmVyc2lvbiI6IjQuNS4wIiwicHVibGlzaCI6InByZS1yZWxlYXNlIiwiaGFzaCI6IjY2MTBiNWJmM2JlNTI3OGY4ZGQ2ZjlhNjkyNjczOGQ3ZDVkNWQyNjJlZjNmNDhjYjM1ZGM5MTZhYTEwMmRkNzEiLCJ1c2VySWQiOm51bGwsInRva2VuSWQiOiIyY2IwYzhmNC05NzA4LTQ3YTgtYjBmZC05ZWQ1MzlmY2M4NDAiLCJpYXQiOjE3MjYzMDcyMzcsImV4cCI6MTc0MzM3OTIwMH0.AuKRlsQQr8rrRNlW3hSKl3BLYciHV7YfA8fTRL3Gxm-dORmBmvbRtzzUnjJgzHbM8gvxQUsBlLesll_w_P58mJQ8hbV1m47SyuxG1N0Kt30Y51yaXe4fWsSnQIqI2zeeSQJRKXX_odf4o7OqaUFWJsOpiQ_SbXJJSmglwVs6QQ494w5H_oePbeXr5NjqXcLeC8Ri1lGE_xwUvMt4ElhBiKZ2SSp3sUki31w-j5zWzCkQ5wVt0rQY5UQeYB_Y4AiMCOqiNorSUEnEDj1No7BZq4EKAizh2jqASiwNAp58a15SJlFXxojFWHKDNnRqe8leANDfIN1dnBWINNTBRXG9Xw
```
<p align="center">
<img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_00_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>02. Set for the Assistant: <font color="red">New feature is available.</font></summary>
&nbsp;

The command "kudos-gpt: show configuration" is available to set values below for the Assistant.

- Flowise API Key
  - example: `FK9DVbyGQYRcs9uv9RqCGVuGpxqcL+pcXj/XhA494o4=`
- Flowise URL
  - example: `http://localhost:3000/api/v1`
- Flowise ChatFlow ID
  - example: `00000000-0000-0000-0000-000000000000`
- Temp Folder
  - example: `/var/tmp`
- Messages
  - clipboard
    - example: `The code:`
  - progress
    - example: `inquiring...`
  - bugAssessment
    - example: `Find the bugs in the code, and show the improvements as the improved code.`
  - vulnerabilityAssessment
    - example: `Find and address vulnerabilities in the code, and show the improvements as the improved code.`
  - speedEnhancement
    - example: `Diagnose if code speed improvement is possible, and show the improvements as the improved code.`
  - etcEnhancement
    - example: `Diagnose if any other improvements are possible, and show the improvements as the improved code.`
  - makeComment
    - example: `Add comments for code review to the class, methods, and all lines of code as the improved code.`
  - makeTest
    - example: `Make tests for the code.`
  - terminal
    - example: `Here are the results. Let me know if any corrections are needed and provide suggestions for improvement.`
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png"/>
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_3.png"/>
</p>
</details>
&nbsp;

<details>
<summary>03. Set for the Copilot:</summary>
The command "kudos-gpt: show configuration" is available to set values below for the Copilot.

- Services
  - example: `Ollama`
- Host
  - example: `http://127.0.0.1:11434`
- Model
  - example: `deepseek-coder:1.3b-base-q4_1`
- FIM
  - example: `starcoder`
- num_predict
  - example: `10`
- temperature
  - example: `0.1`

<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png"/>
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_4.png"/>
</p>
</details>

</details>


<details>
<summary><font size=5>ver 4.4.0</font></summary>
&nbsp;
<details>
 <summary>01. Set the token:</summary>
</br>
To enable the kudos-gpt, the token below needs to be set to the Setting / kudos-gpt / 08 Kudos GPT Toen. To enable setting this value, the VSCode has to be restarted.
</br>
</br>
<font color="red">kudo-gpt token for pre-release, it will be working until 2024-09-30.</font>

```text
eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJwcm9kdWN0Ijoia3Vkb3MtZ3B0IiwidmVyc2lvbiI6IjQuMy4wIiwicHVibGlzaCI6InByZS1yZWxlYXNlIiwiaGFzaCI6ImYzM2VjZjFiZWNlOTk1MGFhZGUzYzQxMTAwODM1Y2MzYmFmYWU0YjU1ZjMxNTdhZTUxNzAyYjI5ZjI1OGNjYmUiLCJ1c2VySWQiOm51bGwsInRva2VuSWQiOiIwZmIyZDE4MS05ZTFkLTQ0MTAtODYxNy01N2U4ODg3OGI5ODYiLCJpYXQiOjE3MTkyMDQ2MDIsImV4cCI6MTcyNzY1NDQwMH0.HhBu87zAdCajtxYKWcl6xNiPYzod9BWAUYnNKUwnBhc_2rOx5z7cb1yR16_MNzTTIQ26NCwl_PXUcYvqsmEwbCzvOsmDwEJV4TYXC_NO209VI5SAhzSGC5mAQdXVcWcUFhQkanzXfORlofauYq5kiWcl_wivod3AdleFmGJRXNjZ2y4uBn5Yf9o0WKqc1wvwobpBY4YXxf5UxgcclRhUgIk9r_PKeaAL0Yq26Z7LTgUm7V1gZ5jpneFA0goxuhKFcJBZcv_L9GvM2cQWAH9vsq6m5JHrwzY_FfG7NPKf_qEyfXbz5URzzH_FjkhLt_QI35q2vD-5oIi_BIpNIKHg1g
```
<p align="center">
<img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_00_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>02. Set for the Assistant:</summary>
&nbsp;

The command "kudos-gpt: show configuration" is available to set values below for the Assistant.

- Flowise URL
  - example: `http://localhost:3000/api/v1`
- Flowise ChatFlow ID
  - example: `00000000-0000-0000-0000-000000000000`
- Temp Folder
  - example: `/var/tmp`
- Messages
  - clipboard
    - example: `The code:`
  - progress
    - example: `inquiring...`
  - bugAssessment
    - example: `Find the bugs in the code, and show the improvements as the improved code.`
  - vulnerabilityAssessment
    - example: `Find and address vulnerabilities in the code, and show the improvements as the improved code.`
  - speedEnhancement
    - example: `Diagnose if code speed improvement is possible, and show the improvements as the improved code.`
  - etcEnhancement
    - example: `Diagnose if any other improvements are possible, and show the improvements as the improved code.`
  - makeComment
    - example: `Add comments for code review to the class, methods, and all lines of code as the improved code.`
  - makeTest
    - example: `Make tests for the code.`
  - terminal
    - example: `Here are the results. Let me know if any corrections are needed and provide suggestions for improvement.`
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png"/>
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_3.png"/>
</p>
</details>
&nbsp;

<details>
<summary>03. Set for the Copilot:</summary>
The command "kudos-gpt: show configuration" is available to set values below for the Copilot.

- Services
  - example: `Ollama`
- Host
  - example: `http://127.0.0.1:11434`
- Model
  - example: `deepseek-coder:1.3b-base-q4_1`
- FIM
  - example: `starcoder`
- num_predict
  - example: `10`
- temperature
  - example: `0.1`

<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png"/>
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_4.png"/>
</p>

</details>
</details>
&nbsp;



<details>
<summary><font size=5>ver 4.3.0</font></summary>
&nbsp;
<details>
 <summary>01. Set the token: <font color="red">New feature is available.</font></summary>
</br>
To enable the kudos-gpt, the token below needs to be set to the Setting / kudos-gpt / 08 Kudos GPT Toen. To enable setting this value, the VSCode has to be restarted.
</br>
</br>
<font color="red">kudo-gpt token for pre-release, it will be working until 2024-09-30.</font>

```text
eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJwcm9kdWN0Ijoia3Vkb3MtZ3B0IiwidmVyc2lvbiI6IjQuMy4wIiwicHVibGlzaCI6InByZS1yZWxlYXNlIiwiaGFzaCI6ImYzM2VjZjFiZWNlOTk1MGFhZGUzYzQxMTAwODM1Y2MzYmFmYWU0YjU1ZjMxNTdhZTUxNzAyYjI5ZjI1OGNjYmUiLCJ1c2VySWQiOm51bGwsInRva2VuSWQiOiIwZmIyZDE4MS05ZTFkLTQ0MTAtODYxNy01N2U4ODg3OGI5ODYiLCJpYXQiOjE3MTkyMDQ2MDIsImV4cCI6MTcyNzY1NDQwMH0.HhBu87zAdCajtxYKWcl6xNiPYzod9BWAUYnNKUwnBhc_2rOx5z7cb1yR16_MNzTTIQ26NCwl_PXUcYvqsmEwbCzvOsmDwEJV4TYXC_NO209VI5SAhzSGC5mAQdXVcWcUFhQkanzXfORlofauYq5kiWcl_wivod3AdleFmGJRXNjZ2y4uBn5Yf9o0WKqc1wvwobpBY4YXxf5UxgcclRhUgIk9r_PKeaAL0Yq26Z7LTgUm7V1gZ5jpneFA0goxuhKFcJBZcv_L9GvM2cQWAH9vsq6m5JHrwzY_FfG7NPKf_qEyfXbz5URzzH_FjkhLt_QI35q2vD-5oIi_BIpNIKHg1g
```

<p align="center">
<img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_00_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>02. Set for the Assistant:</summary>
&nbsp;

The command "kudos-gpt: show configuration" is available to set values below for the Assistant.

- Flowise URL
  - example: `http://localhost:3000/api/v1`
- Flowise ChatFlow ID
  - example: `00000000-0000-0000-0000-000000000000`
- Temp Folder
  - example: `/var/tmp`
- Messages
  - clipboard
    - example: `The code:`
  - progress
    - example: `inquiring...`
  - bugAssessment
    - example: `Find the bugs in the code, and show the improvements as the improved code.`
  - vulnerabilityAssessment
    - example: `Find and address vulnerabilities in the code, and show the improvements as the improved code.`
  - speedEnhancement
    - example: `Diagnose if code speed improvement is possible, and show the improvements as the improved code.`
  - etcEnhancement
    - example: `Diagnose if any other improvements are possible, and show the improvements as the improved code.`
  - makeComment
    - example: `Add comments for code review to the class, methods, and all lines of code as the improved code.`
  - makeTest
    - example: `Make tests for the code.`
  - terminal
    - example: `Here are the results. Let me know if any corrections are needed and provide suggestions for improvement.`
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png"/>
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_3.png"/>
</p>
</details>
&nbsp;

<details>
<summary>03. Set for the Copilot:</summary>
The command "kudos-gpt: show configuration" is available to set values below for the Copilot.

- Services
  - example: `Ollama`
- Host
  - example: `http://127.0.0.1:11434`
- Model
  - example: `deepseek-coder:1.3b-base-q4_1`
- FIM
  - example: `starcoder`
- num_predict
  - example: `10`
- temperature
  - example: `0.1`

<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png"/>
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_4.png"/>
</p>

</details>
</details>
&nbsp;

<details>
<summary><font size=5>ver 4.2.0</font></summary>
&nbsp;
<details>
 <summary>01. Set the token: <font color="red">New feature is available.</font></summary>
</br>
To enable the kudos-gpt, the token below needs to be set to the Setting / kudos-gpt / 08 Kudos GPT Toen. To enable setting this value, the VSCode has to be restarted.
</br>
</br>
<font color="red">kudo-gpt token for pre-release, it will be working until 2024-08-31.</font>

```text
eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJwcm9kdWN0Ijoia3Vkb3MtZ3B0IiwidmVyc2lvbiI6IjQuMi4wIiwicHVibGlzaCI6InByZS1yZWxlYXNlIiwiaGFzaCI6Ijk4MjIyNTEyMjYxYzUxZWEzZDlkMTlmOGQ3ODkwNmY1N2Q5MzllYjVhM2Q1YWY1MTlmY2ZlOGQ2OTBmOTBmNzgiLCJ1c2VySWQiOm51bGwsInRva2VuSWQiOiJhZWJhN2E0Zi0yYWU5LTRjYTktOTY3Zi0yMmZmZDUzYjFlODQiLCJpYXQiOjE3MTIyNDQyNDMsImV4cCI6MTcyNTA2MjQwMH0.tqRRWGWoNzvc_9NqJQd6UGVnqwCw2emxs_A4wAWiJKK5U7v7URMSInHeycE3n7OAfxxlbFmbzKcHrdCh2Qh99KOP0rCM-5X717p_X2_2feWa21HtLYXXpSLG0ehhdp8sUNZAkK8IU57oqjqQvOZNbt4Tv9MLLsP657y2y9m9eFZPpUR2l2QPiVR-ASnQIZYTmoqyLrx_puZTvb3T8dkUDDhl8MZBaDN3eeFtGPqnR4OXGEOmMlw82EpZiF8emvV4Zo6Rr0cVUsEiR7fSxMpDNN9TdX2k97YBkyX3-YoPffASaA4bpAeLNxBtzoPTNWYqrtcbP-UcBTvGxQhZzokc6gs
```

<p align="center">
<img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_00_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>02. Set for the Assistant:</summary>
&nbsp;

The command "kudos-gpt: show configuration" is available to set values below for the Assistant.

- Flowise URL
  - example: `http://localhost:3000/api/v1`
- Flowise ChatFlow ID
  - example: `00000000-0000-0000-0000-000000000000`
- Temp Folder
  - example: `/var/tmp`
- Messages
  - clipboard
    - example: `The code:`
  - progress
    - example: `inquiring...`
  - bugAssessment
    - example: `Find the bugs in the code, and show the improvements as the improved code.`
  - vulnerabilityAssessment
    - example: `Find and address vulnerabilities in the code, and show the improvements as the improved code.`
  - speedEnhancement
    - example: `Diagnose if code speed improvement is possible, and show the improvements as the improved code.`
  - etcEnhancement
    - example: `Diagnose if any other improvements are possible, and show the improvements as the improved code.`
  - makeComment
    - example: `Add comments for code review to the class, methods, and all lines of code as the improved code.`
  - makeTest
    - example: `Make tests for the code.`
  - terminal
    - example: `Here are the results. Let me know if any corrections are needed and provide suggestions for improvement.`
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png"/>
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_3.png"/>
</p>
</details>
&nbsp;

<details>
<summary>03. Set for the Copilot:</summary>
The command "kudos-gpt: show configuration" is available to set values below for the Copilot.

- Services
  - example: `Ollama`
- Host
  - example: `http://127.0.0.1:11434`
- Model
  - example: `deepseek-coder:1.3b-base-q4_1`
- FIM
  - example: `starcoder`
- num_predict
  - example: `10`
- temperature
  - example: `0.1`

<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png"/>
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_4.png"/>
</p>

</details>
</details>
&nbsp;

<details>
<summary><font size=5>ver 4.1.0</font></summary>
&nbsp;
<details>
 <summary>01. Set the token: <font>New feature is available.</font></summary>
</br>
To enable the kudos-gpt, the token below needs to be set to the Setting / kudos-gpt / 08 Kudos GPT Toen. To enable setting this value, the VSCode has to be restarted.
</br>
</br>
<font color="red">kudo-gpt token for pre-release, it will be working until 2024-08-31.</font>

```text
eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJwcm9kdWN0Ijoia3Vkb3MtZ3B0IiwidmVyc2lvbiI6IjQuMS4wIiwicHVibGlzaCI6InByZS1yZWxlYXNlIiwiaGFzaCI6IjhjMTEwNjU5M2M1MDc2OTBlZTAzZGViM2M4ZGRmNmE3ZTE5MjYzMDc5MzU2MDQ3M2M0N2EzZDJkYjAxNWMwYTMiLCJ1c2VySWQiOm51bGwsInRva2VuSWQiOiIyYzYxYTBiYi1jMDk3LTQ2YTAtODNmZS05YmIwYWFhNTZiMWMiLCJpYXQiOjE3MTA1MTc2MDEsImV4cCI6MTcyNTA2MjQwMH0.m3CC5LgRSO50gtmGkOAPJ2JUL3oQBuTkeJAPJRgxap4OdzSSaRQ5IHCrlBb4qKpm6BkEUWCodTo_yZEUCQ4q4zqxkS1eh0J3gfEhPPEAiyRZaKqswZlrd3DprjWBVz_9-znmMT84DayO4oSB_yWvHXbB1HvMRIP5ViHvT1bBh3lvElaLkmz0K1mLLxNMs40n-b3DN4hGxRUFxxWdSFtl2SKsRtzqLh2gBX9UWpn6TpPtj8HNo3UmKyP6hNEpmphY9jrl8xRGQZdC8YUAL1eqSPsAGCWDBmBVVJX45AhOMi2eXP4TvCRIWK7JKfnMAa0AErxie9C_kLrXIEK42Ye2bg
```

<p align="center">
<img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_00_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>02. Set for the Assistant: <font>New feature is available.</font></summary>
&nbsp;

The command "kudos-gpt: show configuration" is available to set values below for the Assistant.

- Flowise URL
  - example: `http://localhost:3000/api/v1`
- Flowise ChatFlow ID
  - example: `00000000-0000-0000-0000-000000000000`
- Temp Folder
  - example: `/var/tmp`
- Messages
  - clipboard
    - example: `The code:`
  - progress
    - example: `inquiring...`
  - bugAssessment
    - example: `Find the bugs in the code, and show the improvements as the improved code.`
  - vulnerabilityAssessment
    - example: `Find and address vulnerabilities in the code, and show the improvements as the improved code.`
  - speedEnhancement
    - example: `Diagnose if code speed improvement is possible, and show the improvements as the improved code.`
  - etcEnhancement
    - example: `Diagnose if any other improvements are possible, and show the improvements as the improved code.`
  - makeComment
    - example: `Add comments for code review to the class, methods, and all lines of code as the improved code.`
  - makeTest
    - example: `Make tests for the code.`
  - terminal
    - example: `Here are the results. Let me know if any corrections are needed and provide suggestions for improvement.`
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png"/>
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_3.png"/>
</p>
</details>
&nbsp;

<details>
<summary>03. Set for the Copilot: <font>New feature is available.</font></summary>
The command "kudos-gpt: show configuration" is available to set values below for the Copilot.

- Services
  - example: `Ollama`
- Host
  - example: `http://127.0.0.1:11434`
- Model
  - example: `deepseek-coder:1.3b-base-q4_1`
- FIM
  - example: `starcoder`
- num_predict
  - example: `10`
- temperature
  - example: `0.1`

<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png"/>
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_4.png"/>
</p>

</details>
</details>
&nbsp;



<details>
<summary><font size=5>ver 4.0.0</font></summary>
<details>
<summary>00. Sample a Flowise ChatFlow and a docker-compose: <font color="red">New feature is available.</font></summary>
The kudos-gpt expects to be used the Chat Memory on the [Flowise](https://github.com/FlowiseAI/Flowise?tab=readme-ov-file). So let me show a sample of it as files below.
</br>
[kudos-gpt with llama2(ollama)](https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_with_llama2(ollama)_Chatflow.json)
[docker-compose.yml](https://github.com/akudo7/kudos-gpt/raw/HEAD/docker-compose.yml)
</br>
<p align="center">
<img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.0.0_1.png" />
</p>
</details>
&nbsp;
<details>
 <summary>01. Set the token: <font color="red">New feature is available.</font></summary>
</br>
To enable the kudos-gpt, the token below needs to be set to the Setting / kudos-gpt / 08 Kudos GPT Toen. To enable setting this value, the VSCode has to be restarted.
</br>
</br>
<font color="red">kudo-gpt token for pre-release, it will be working until 2024-08-31.</font>

```text
eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJwcm9kdWN0Ijoia3Vkb3MtZ3B0IiwidmVyc2lvbiI6IjQuMC4wIiwicHVibGlzaCI6InByZS1yZWxlYXNlIiwiaGFzaCI6IjExZDYzZmRhZGVmMjZlNDk3MzMzOTA2MWQ5MTA0OGFjY2I5MzlhM2I3OWI3NzM1MjI0YWExY2JjMTlhNDNjYjkiLCJ1c2VySWQiOm51bGwsInRva2VuSWQiOiJkZGNjOTBhYy0yYjEwLTRiZjktOTNlMS1hZTMwMTRlMDhlYzAiLCJpYXQiOjE3MDkzNjAxODcsImV4cCI6MTcyNTA2MjQwMH0.n6e872xDZyy9kRJNI5GL3SSi3Ogcxpcjc-qK_Q8GdBrDc9XZGAl381YFHgzCWG4uJOBHj0DaYSRPRHnR7GE3_fY0uKrtuvpxeoc4q-mvNg7zjI6D7zwRxGBvKz-fQaven-ba724HUkc8xbt64vzsoQt5gc1jj0DKH-9D_jhKljE6IVtXkTryrRiT8bs6BIl0jboqiVAuYEbthVaWDQttQ5XFH1OMZ0IM0SaoPpV93eEYpLagOOKrXtsmXFT8kPxCBTQecrESCz6ie2tVdmRZsQlcN8n7Mupev8dMWSJU6E_4SaTrHkTPnlox6VddQP0tOmbz5GL2o2lFi_4VFnrjrg
```

<p align="center">
<img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_00_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>02. Set the Flowise URL and a ChatFlowId: <font color="red">New feature is available.</font></summary>
&nbsp;

To use the Flowise, some values below have to be set.

- Setting / kudos-gpt / Flowise ChatFlow ID
  - 00000000-0000-0000-0000-000000000000
- Setting / kudos-gpt / Flowise URL
  - http://localhost:3000/api/v1

To enable these values, the VSCode has to be restarted.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_70_1.png" />
</p>
</details>
&nbsp;


<details>
<summary>03. Adjustment of the messages of the buttons: <font color="red">New feature is available.</font></summary></summary>

To change the messages of the buttons, some values below have to be edited in settings.json.

- Setting / kudos-gpt / Messages

    ```json
    "kudos-gpt.messages": {
        "clipboard": "The code:",
        "progress": "inquiring...",
        "bugAssessment": "Find the bugs in the code, and show the improvements as the improved code.",
        "vulnerabilityAssessment": "Find and address vulnerabilities in the code, and show the improvements as the improved code.",
        "speedEnhancement": "Diagnose if code speed improvement is possible, and show the improvements as the improved code.",
        "etcEnhancement": "Diagnose if any other improvements are possible, and show the improvements as the improved code.",
        "makeComment": "Add comments for code review to the class, methods, and all lines of code as the improved code.",
        "makeTest": "Make tests for the code.",
        "terminal": "Here are the results. Let me know if any corrections are needed and provide suggestions for improvement."
    },
    ```

    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_03_1.png" />
    </p>

</details>
&nbsp;

<details>
<summary>04. Adjustment of the temporary folder:</summary>

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

<details>
<summary>05. Adjustment of the Copilot: </summary>

- Setting / kudos-gpt / 16 Copilot Services
  - Your LLM Host URL
  - example: `Ollama`
- Setting / kudos-gpt / 17 Copilot Host
  - Your Ollama Host URL
  - example: `http://127.0.0.1:11434`
- Setting / kudos-gpt / 18 Copilot Model
  - Your Copilot Model
  - example: `deepseek-coder:1.3b-base-q4_1`
- Setting / kudos-gpt / 19 Copilot FIM
  - Your Copilot FIM
  - example: `starcoder`
- Setting / kudos-gpt / 20 Copilot Options

    ```json
    "kudos-gpt.20CopilotOptions": {
        "num_predict": 10,
        "temperature": 0.1
    },
    ```

    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_60_1.png" />
    </p>
To enable these values, the VSCode has to be restarted.

</details>
&nbsp;

</details>
&nbsp;


<details>
<summary><font size=5>ver 3.0.0</font></summary>
<details>
 <summary>01. Set the token: <font color="red">New feature is available.</font></summary>
</br>
To enable the kudos-gpt, the token below needs to be set to the Setting / kudos-gpt / 08 Kudos GPT Toen. To enable setting this value, the VSCode has to be restarted.
</br>
</br>
<font color="red">kudo-gpt token for pre-release, it will be working until 2024-12-31.</font>

```text
eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJwcm9kdWN0Ijoia3Vkb3MtZ3B0IiwidmVyc2lvbiI6IjMuMC4wIiwicHVibGlzaCI6InByZS1yZWxlYXNlIiwiaGFzaCI6ImZjNWJlM2NkMWUzMTZlMDRlODRhMGZkMTg3NjUwNGNlODdlNDhiODIyZTI3ODE0ZmEwNTk2OGViMGQwYmMxMzQiLCJ1c2VySWQiOm51bGwsInRva2VuSWQiOiI4YTFmMzhhYS1hY2NhLTRhMGEtOGJlYS1hYzlmNTUyZDVmODciLCJpYXQiOjE3MDU0ODExMjEsImV4cCI6MTczNTYwMzIwMH0.NbysFXW2j-OLIQsb5w-KSsL7s9mFRpaodeLLjqXvzKQ2v1z6XpY_DPyBocbD_V-b2w51uLhchrDttaYEVERL_icqlSJg8W_oeewFWD1Yn2Udoc9PQOi1-bk9A2cfdY63rGunJ62bGZdlL2MI3Jtwg3VrjNWBKVysSIJqBvVXaH7vjXYtp2I5Jq1f9P1lEQ26PWonKF4lA_nFThhZEsXvkc-_6vjyiW3Pd6z2Lw9PLT_8DdbvHnyzpNy5KCSP7EC4en_uo6FDo2hPBef0owjBRzbzoK7BNISPRRH4mZ0FxuoTatAtqcof4o9XPaZLZU79KJcalfk429WpVv5Hx0egDA
```

<p align="center">
<img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_00_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>02. Choose the OpenAI, Azure OpenAI, GPT4ALL or Ollama: <font color="red">New feature is available.</font></summary>
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
  - gpt-4-1106-preview

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
&nbsp;
<details>
<summary>GPT4ALL</summary>

To use the GPT4ALL, some values below have to be set. They should be comfirmed working with the GPT4ALL <a href="https://github.com/nomic-ai/gpt4all?tab=readme-ov-file#chat-client">Chat Client</a> beforehands.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/gpt4all_device.png" />
    </p>
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/gpt4all_env.png" />
    </p>

- Setting / kudos-gpt / 01 Services
  - GPT4ALL
- Setting / kudos-gpt / 10 GPT4ALL Device
  - cpu
  - gpt
  - amd
  - nvidia
  - intel
  - example: `cpu`
- Setting / kudos-gpt / 11 GPT4ALL Model
  - Your GPT4ALL Model
  - example: `mistral-7b-openorca.Q4_0.gguf`
- Setting / kudos-gpt / 12 GPT4ALL Model Folder
  - Your GPT4ALL Model Folder `as full path`
  - example: `/Users/akirakudo/Library/Application Support/nomic.ai/GPT4All`
- Setting / kudos-gpt / 13 GPT4ALL Chat Options

    ```json
        "kudos-gpt.13gpt4allChatOptions": {
            "tokensSize": 4000,
            "temp": 0.7,
            "topK": 40,
            "topP": 0.4,
            "repeatPenalty": 1.18,
            "repeatLastN": 64,
            "nBatch": 8,
            "nPredict": 1000,
            "systemPromptTemplate": "%1"
        },
    ```

To enable these values, the VSCode has to be restarted.
</details>
&nbsp;
<details>
<summary><font color="red">Ollama</font></summary>

To use the Ollama, some values below have to be set. They should be comfirmed working with the Ollama <a href="https://github.com/ollama-webui/ollama-webui">Chat Client</a> beforehands.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/ollama-ui_1.png" />
    </p>
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/ollama-ui_2.png" />
    </p>
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/ollama-ui_3.png" />
    </p>
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/ollama-ui_4.png" />
    </p>

- Setting / kudos-gpt / 01 Services
  - Ollama
- Setting / kudos-gpt / 14 Ollama Host
  - Your Ollama Host URL
  - example: `http://127.0.0.1:11434`
- Setting / kudos-gpt / 15 Ollama Model
  - Your Ollama Model
  - example: `llama2`

    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/ollama-ui_5.png" />
    </p>

To enable these values, the VSCode has to be restarted.
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
&nbsp;

<details>
<summary>04. Adjustment of the messages of the buttons:</summary>

To change the messages of the buttons, some values below have to be edited in settings.json.

- Setting / kudos-gpt / Messages

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
&nbsp;

<details>
<summary>06. Adjustment of the Copilot:  <font color="red">New feature is available.</font></summary>

- Setting / kudos-gpt / 16 Copilot Services
  - Your LLM Host URL
  - example: `Ollama`
- Setting / kudos-gpt / 17 Copilot Host
  - Your Ollama Host URL
  - example: `http://127.0.0.1:11434`
- Setting / kudos-gpt / 18 Copilot Model
  - Your Copilot Model
  - example: `deepseek-coder:1.3b-base-q4_1`
- Setting / kudos-gpt / 19 Copilot FIM
  - Your Copilot FIM
  - example: `starcoder`
- Setting / kudos-gpt / 20 Copilot Options

    ```json
    "kudos-gpt.20CopilotOptions": {
        "num_predict": 10,
        "temperature": 0.1
    },
    ```

    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_60_1.png" />
    </p>
To enable these values, the VSCode has to be restarted.

</details>
&nbsp;

</details>
&nbsp;



<details>
<summary><font size=5>ver 2.2.0</font></summary>
<details>
 <summary>01. Set the token: <font color="red">New feature is available.</font></summary>
</br>
To enable the kudos-gpt, the token below needs to be set to the Setting / kudos-gpt / 08 Kudos GPT Toen. To enable setting this value, the VSCode has to be restarted.
</br>
</br>
<font color="red">kudo-gpt token for pre-release, it will be working until 2024-12-31.</font>

```text
eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9.eyJwcm9kdWN0Ijoia3Vkb3MtZ3B0IiwidmVyc2lvbiI6IjIuMi4wIiwicHVibGlzaCI6InByZS1yZWxlYXNlIiwiaGFzaCI6ImVmODZkNWRiNDdhNGQ4YTVmNDM0ZDNlZDhiODJlZmYxNWEyYjg5ZjhkNjBlNzcxZGNiNzMyNTU0MzcyZTU0ZjIiLCJ1c2VySWQiOm51bGwsInRva2VuSWQiOiI1MWE4OGFlZi1kYTE1LTQ4ZDEtOTIwNC02NzBiNjZmZWZhYmYiLCJpYXQiOjE3MDQzMjg1ODIsImV4cCI6MTczNTYwMzIwMH0.RkFs2a1S19-KFS6p4ptuupHLQZyb9Jqg4inY7z8RLPmoiCfGQ1z4ut3qIv8b652WzN1TQFoGVxHaiQRlx1GKQvcSa0E6EwkItzVB1hnY4Jk14h6ZA5kJYgU0lXPIRlQ9meMML7PaoylykPgpPN5QhydGN1cN7MEwYx-v6RuqEAiqjyGArmihUPKcHBAS7im4GlnKeHi0IGHRVAy9IhZ9VPCXkh05Raa4d1J4cX-F-qyKLB0Kt_hBnzDKbCjggWL0pkPhSfPSrhOgC89fNLnnGKxvdQQicT6s_g8d7Hybh2XDwOqCpx3qTNsM_AaBOgcqAxG19SwenSOKJFRRFbhgfQ
```

<p align="center">
<img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_00_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>02. Choose the OpenAI, Azure OpenAI or GPT4ALL: <font color="red">New feature is available.</font></summary>
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
  - gpt-4-1106-preview

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
&nbsp;
<details>
<summary><font color="red">GPT4ALL</font></summary>

To use the GPT4ALL, some values below have to be set. They should be comfirmed working with the GPT4ALL <a href="https://github.com/nomic-ai/gpt4all?tab=readme-ov-file#chat-client">Chat Client</a> beforehands.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/gpt4all_device.png" />
    </p>
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/gpt4all_env.png" />
    </p>

- Setting / kudos-gpt / 01 Services
  - GPT4ALL
- Setting / kudos-gpt / 10 GPT4ALL Device
  - cpu
  - gpt
  - amd
  - nvidia
  - intel
  - example: `cpu`
- Setting / kudos-gpt / 11 GPT4ALL Model
  - Your GPT4ALL Model
  - example: `mistral-7b-openorca.Q4_0.gguf`
- Setting / kudos-gpt / 12 GPT4ALL Model Folder
  - Your GPT4ALL Model Folder `as full path`
  - example: `/Users/akirakudo/Library/Application Support/nomic.ai/GPT4All`
- Setting / kudos-gpt / 13 GPT4ALL Chat Options

    ```json
        "kudos-gpt.13gpt4allChatOptions": {
            "tokensSize": 4000,
            "temp": 0.7,
            "topK": 40,
            "topP": 0.4,
            "repeatPenalty": 1.18,
            "repeatLastN": 64,
            "nBatch": 8,
            "nPredict": 1000,
            "systemPromptTemplate": "%1"
        },
    ```

To enable these values, the VSCode has to be restarted.
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

- Setting / kudos-gpt / Messages

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
&nbsp;
</details>
&nbsp;

<details>
<summary><font size=5>ver 2.1.0</font></summary>
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

<summary><font color="red" size=5>ver 5.0.0</font></summary>
<details>
<summary>01. Configuration: </summary>

- Configuration
  - After loading the kudos-gpt successfully, the `kudos-gpt: show configuration` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png" />
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.5.0_2.png" />
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_4.png" />
    </p>
</details>
&nbsp;
<details>
<summary>02. Turn On/Off: </summary>

- Assistans
  - After loading the kudos-gpt successfully, the `kudos-gpt: Assistants On/Off` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_1.png" />
    </p>
    So the plus icon on the left will be available for creating/opening a discussion.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_2.png" />
    </p>
- Copilot
  - After loading the kudos-gpt successfully, the `kudos-gpt: Copilot On/Off` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_3.png" />
    </p>
    So the inputing the return key on the code will be available for asking some candidate codes to a LLM.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v3.0.0_1.gif" />
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
<summary>04. Have a discussion by asking image: </summary>
To ask your question about an image in a discussion, the `Asking image` button is available.
Note that, input a question is required before push it.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.4.0_1.gif"/>
</p>
</details>
&nbsp;
<details>
<summary>05. Have a discussion with templates:</summary>

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
<summary>06. Create a message from a terminal:</summary>

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
<summary>07. Inject a discussion: </summary>

To Inject a chat from Flowise is available with the injection icon `Chat injection`. And also available to keep continue the conversation after entering a chatId is success.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.3.0_1.gif" />
</p>
</details>
&nbsp;
<details>
<summary>08. Save a discussion: </summary>

To Save a log in a discussion is available with the pencil icon `JSON Export`. It will be created a new JSON file as an `opening file + .{Flowise ChatFlowId}.json`. It will be imported automatically when an original closed file is opened.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_11_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>09. Delete a discussion: </summary></summary>

To delete a discussion, the cross icon `del thread` is available. It will also delete a thread on the Flowise Chat Mdemory.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_07_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>10. Compare/update an active text editor with a message</summary>

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
<summary>11. l10n supporting</summary>

- English
- Japanese

</details>
&nbsp;
<details>
<summary>12. Devin<font color="red"> New feature is available.</font></summary>

Supported Devin feature
  - Available to import XMLs which are exported by the Bolt.new system promopt.
    - See in detail of the original prompt at the "https://github.com/stackblitz/bolt.new/blob/main/app/lib/.server/llm/prompts.ts".
      - Recommend to change it for fitting with your environment.
    - boltArtifact and bolt_file_modifications are supported.
    - Samples
      - [System Prompt](https://github.com/akudo7/kudos-gpt/raw/HEAD/bolt_new-system-prompt.txt) 
      - [artifact.xml](https://github.com/akudo7/kudos-gpt/raw/HEAD/artifact.xml) 
      - [modifications.xml](https://github.com/akudo7/kudos-gpt/raw/HEAD/modifications.xml) 
  <p align="center">
  <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v5.0.0_1.gif"/>
  <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v5.0.0_2.gif"/>
  </p>


</details>

<details>
<summary><font size=5>ver 4.6.0</font></summary>
<details>
<summary>01. Configuration: </summary>

- Configuration
  - After loading the kudos-gpt successfully, the `kudos-gpt: show configuration` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png" />
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.5.0_2.png" />
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_4.png" />
    </p>
</details>
&nbsp;
<details>
<summary>02. Turn On/Off: </summary>

- Assistans
  - After loading the kudos-gpt successfully, the `kudos-gpt: Assistants On/Off` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_1.png" />
    </p>
    So the plus icon on the left will be available for creating/opening a discussion.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_2.png" />
    </p>
- Copilot
  - After loading the kudos-gpt successfully, the `kudos-gpt: Copilot On/Off` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_3.png" />
    </p>
    So the inputing the return key on the code will be available for asking some candidate codes to a LLM.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v3.0.0_1.gif" />
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
<summary>04. Have a discussion by asking image: </summary>
To ask your question about an image in a discussion, the `Asking image` button is available.
Note that, input a question is required before push it.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.4.0_1.gif"/>
</p>
</details>
&nbsp;
<details>
<summary>05. Have a discussion with templates:</summary>

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
<summary>06. Create a message from a terminal:</summary>

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
<summary>07. Inject a discussion: </summary>

To Inject a chat from Flowise is available with the injection icon `Chat injection`. And also available to keep continue the conversation after entering a chatId is success.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.3.0_1.gif" />
</p>
</details>
&nbsp;
<details>
<summary>08. Save a discussion: </summary>

To Save a log in a discussion is available with the pencil icon `JSON Export`. It will be created a new JSON file as an `opening file + .{Flowise ChatFlowId}.json`. It will be imported automatically when an original closed file is opened.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_11_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>09. Delete a discussion: </summary></summary>

To delete a discussion, the cross icon `del thread` is available. It will also delete a thread on the Flowise Chat Mdemory.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_07_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>10. Compare/update an active text editor with a message</summary>

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
<summary>11. l10n supporting</summary>

- English
- Japanese

</details>
</details>
&nbsp;

<details>
<summary><font size=5>ver 4.5.0</font></summary>
<details>
<summary>01. Configuration: <font color="red">New feature is available.</font></summary>

- Configuration
  - After loading the kudos-gpt successfully, the `kudos-gpt: show configuration` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png" />
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.5.0_2.png" />
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_4.png" />
    </p>
</details>
&nbsp;
<details>
<summary>02. Turn On/Off: </summary>

- Assistans
  - After loading the kudos-gpt successfully, the `kudos-gpt: Assistants On/Off` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_1.png" />
    </p>
    So the plus icon on the left will be available for creating/opening a discussion.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_2.png" />
    </p>
- Copilot
  - After loading the kudos-gpt successfully, the `kudos-gpt: Copilot On/Off` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_3.png" />
    </p>
    So the inputing the return key on the code will be available for asking some candidate codes to a LLM.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v3.0.0_1.gif" />
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
<summary>04. Have a discussion by asking image: </summary>
To ask your question about an image in a discussion, the `Asking image` button is available.
Note that, input a question is required before push it.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.4.0_1.gif"/>
</p>
</details>
&nbsp;
<details>
<summary>05. Have a discussion with templates:</summary>

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
<summary>06. Create a message from a terminal:</summary>

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
<summary>07. Inject a discussion: </summary>

To Inject a chat from Flowise is available with the injection icon `Chat injection`. And also available to keep continue the conversation after entering a chatId is success.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.3.0_1.gif" />
</p>
</details>
&nbsp;
<details>
<summary>08. Save a discussion: </summary>

To Save a log in a discussion is available with the pencil icon `JSON Export`. It will be created a new JSON file as an `opening file + .{Flowise ChatFlowId}.json`. It will be imported automatically when an original closed file is opened.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_11_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>09. Delete a discussion: </summary></summary>

To delete a discussion, the cross icon `del thread` is available. It will also delete a thread on the Flowise Chat Mdemory.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_07_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>10. Compare/update an active text editor with a message</summary>

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
<summary>11. l10n supporting</summary>

- English
- Japanese

</details>
</details>

&nbsp;



<details>
<summary><font size=5>ver 4.4.0</font></summary>
<details>
<summary>01. Configuration:</summary>

- Configuration
  - After loading the kudos-gpt successfully, the `kudos-gpt: show configuration` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png" />
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_3.png" />
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_4.png" />
    </p>
</details>
&nbsp;
<details>
<summary>02. Turn On/Off: </summary>

- Assistans
  - After loading the kudos-gpt successfully, the `kudos-gpt: Assistants On/Off` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_1.png" />
    </p>
    So the plus icon on the left will be available for creating/opening a discussion.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_2.png" />
    </p>
- Copilot
  - After loading the kudos-gpt successfully, the `kudos-gpt: Copilot On/Off` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_3.png" />
    </p>
    So the inputing the return key on the code will be available for asking some candidate codes to a LLM.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v3.0.0_1.gif" />
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
<summary>04. Have a discussion by asking image: </summary>
To ask your question about an image in a discussion, the `Asking image` button is available.
Note that, input a question is required before push it.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.4.0_1.gif"/>
</p>
</details>
&nbsp;
<details>
<summary>05. Have a discussion with templates:</summary>

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
<summary>06. Create a message from a terminal:</summary>

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
<summary>07. Inject a discussion: </summary>

To Inject a chat from Flowise is available with the injection icon `Chat injection`. And also available to keep continue the conversation after entering a chatId is success.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.3.0_1.gif" />
</p>
</details>
&nbsp;
<details>
<summary>08. Save a discussion: </summary>

To Save a log in a discussion is available with the pencil icon `JSON Export`. It will be created a new JSON file as an `opening file + .{Flowise ChatFlowId}.json`. It will be imported automatically when an original closed file is opened.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_11_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>09. Delete a discussion: </summary></summary>

To delete a discussion, the cross icon `del thread` is available. It will also delete a thread on the Flowise Chat Mdemory.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_07_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>10. Compare/update an active text editor with a message</summary>

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
<summary>11. l10n supporting</summary>

- English
- Japanese

</details>
</details>

&nbsp;








<details>
<summary><font size=5>ver 4.3.0</font></summary>
<details>
<summary>01. Configuration:</summary>

- Configuration
  - After loading the kudos-gpt successfully, the `kudos-gpt: show configuration` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png" />
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_3.png" />
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_4.png" />
    </p>
</details>
&nbsp;
<details>
<summary>02. Turn On/Off: </summary>

- Assistans
  - After loading the kudos-gpt successfully, the `kudos-gpt: Assistants On/Off` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_1.png" />
    </p>
    So the plus icon on the left will be available for creating/opening a discussion.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_2.png" />
    </p>
- Copilot
  - After loading the kudos-gpt successfully, the `kudos-gpt: Copilot On/Off` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_3.png" />
    </p>
    So the inputing the return key on the code will be available for asking some candidate codes to a LLM.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v3.0.0_1.gif" />
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
<summary>06. Inject a discussion: <font color="red">New feature is available.</font></summary>

To Inject a chat from Flowise is available with the injection icon `Chat injection`. And also available to keep continue the conversation after entering a chatId is success.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.3.0_1.gif" />
</p>
</details>
&nbsp;
<details>
<summary>07. Save a discussion: </summary>

To Save a log in a discussion is available with the pencil icon `JSON Export`. It will be created a new JSON file as an `opening file + .{Flowise ChatFlowId}.json`. It will be imported automatically when an original closed file is opened.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_11_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>08. Delete a discussion: </summary></summary>

To delete a discussion, the cross icon `del thread` is available. It will also delete a thread on the Flowise Chat Mdemory.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_07_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>09. Compare/update an active text editor with a message</summary>

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
<summary>10. l10n supporting</summary>

- English
- Japanese

</details>
</details>
&nbsp;








<details>
<summary><font size=5>ver 4.2.0</font></summary>
<details>
<summary>01. Configuration:</summary>

- Configuration
  - After loading the kudos-gpt successfully, the `kudos-gpt: show configuration` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png" />
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_3.png" />
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_4.png" />
    </p>
</details>
&nbsp;
<details>
<summary>02. Turn On/Off: </summary>

- Assistans
  - After loading the kudos-gpt successfully, the `kudos-gpt: Assistants On/Off` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_1.png" />
    </p>
    So the plus icon on the left will be available for creating/opening a discussion.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_2.png" />
    </p>
- Copilot
  - After loading the kudos-gpt successfully, the `kudos-gpt: Copilot On/Off` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_3.png" />
    </p>
    So the inputing the return key on the code will be available for asking some candidate codes to a LLM.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v3.0.0_1.gif" />
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
<summary>06. Save a discussion: </summary>

To Save a log in a discussion is available with the pencil icon `JSON Export`. It will be created a new JSON file as an `opening file + .{Flowise ChatFlowId}.json`. It will be imported automatically when an original closed file is opened.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_11_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>07. Delete a discussion: </summary></summary>

To delete a discussion, the cross icon `del thread` is available. It will also delete a thread on the Flowise Chat Mdemory.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_07_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>08. Compare/update an active text editor with a message</summary>

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
<summary>09. l10n supporting</summary>

- English
- Japanese

</details>
</details>
&nbsp;








<details>
<summary><font size=5>ver 4.1.0</font></summary>
<details>
<summary>01. Configuration:</summary>

- Configuration
  - After loading the kudos-gpt successfully, the `kudos-gpt: show configuration` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_2.png" />
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_3.png" />
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v4.1.0_4.png" />
    </p>
</details>
&nbsp;
<details>
<summary>02. Turn On/Off: </summary>

- Assistans
  - After loading the kudos-gpt successfully, the `kudos-gpt: Assistants On/Off` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_1.png" />
    </p>
    So the plus icon on the left will be available for creating/opening a discussion.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_2.png" />
    </p>
- Copilot
  - After loading the kudos-gpt successfully, the `kudos-gpt: Copilot On/Off` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_3.png" />
    </p>
    So the inputing the return key on the code will be available for asking some candidate codes to a LLM.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v3.0.0_1.gif" />
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
<summary>06. Save a discussion: </summary>

To Save a log in a discussion is available with the pencil icon `JSON Export`. It will be created a new JSON file as an `opening file + .{Flowise ChatFlowId}.json`. It will be imported automatically when an original closed file is opened.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_11_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>07. Delete a discussion: </summary></summary>

To delete a discussion, the cross icon `del thread` is available. It will also delete a thread on the Flowise Chat Mdemory.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_07_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>08. Compare/update an active text editor with a message</summary>

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
<summary>09. l10n supporting</summary>

- English
- Japanese

</details>
</details>
&nbsp;








<details>
<summary><font size=5>ver 4.0.0</font></summary>
<details>
<summary>01. Turn On/Off: </summary>

- Assistans
  - After loading the kudos-gpt successfully, the `kudos-gpt: Assistants On/Off` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_1.png" />
    </p>
    So the plus icon on the left will be available for creating/opening a discussion.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_2.png" />
    </p>
- Copilot
  - After loading the kudos-gpt successfully, the `kudos-gpt: Copilot On/Off` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_3.png" />
    </p>
    So the inputing the return key on the code will be available for asking some candidate codes to a LLM.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v3.0.0_1.gif" />
    </p>
</details>
&nbsp;
<details>
<summary>02. Have a discussion by asking directly:</summary>
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
<summary>03. Have a discussion with templates:</summary>

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
<summary>04. Create a message from a terminal:</summary>

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
<summary>05. Save a discussion: </summary>

To Save a log in a discussion is available with the pencil icon `JSON Export`. It will be created a new JSON file as an `opening file + .{Flowise ChatFlowId}.json`. It will be imported automatically when an original closed file is opened.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_11_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>06. Delete a discussion: </summary></summary>

To delete a discussion, the cross icon `del thread` is available. It will also delete a thread on the Flowise Chat Mdemory.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_07_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>07. Compare/update an active text editor with a message</summary>

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
<summary>08. l10n supporting</summary>

- English
- Japanese

</details>
</details>
&nbsp;








<details>
<summary><font size=5>ver 3.0.0</font></summary>
<details>
<summary>01. Turn On/Off: <font color="red">New feature is available.</font></summary>

- Assistans
  - After loading the kudos-gpt successfully, the `kudos-gpt: Assistants On/Off` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_1.png" />
    </p>
    So the plus icon on the left will be available for creating/opening a discussion.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_2.png" />
    </p>
- Copilot
  - After loading the kudos-gpt successfully, the `kudos-gpt: Copilot On/Off` has to be executed yourself for turnning it on.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_04_3.png" />
    </p>
    So the inputing the return key on the code will be available for asking some candidate codes to a LLM.
    <p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt.v3.0.0_1.gif" />
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
<summary>06. Save a discussion: </summary>

To Save a log in a discussion is available with the pencil icon `JSON Export`. It will be created a new JSON file as an `opening file + .json` for the Azure OpenAI, and also `opening file + .{model name}.openai.json` that has a threadId and assistantId for the OpenAI.  <font color="red">For the GPT4ALL, `opening file + .{model name}.gpt4all.json`.</font> They will be imported automatically when an original closed file is opened.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_11_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>07. Delete a discussion: </summary></summary>

To delete a discussion, the cross icon `del thread` is available.
<font color="red">NOTE: It is removed from a JSON file, and also deleting the thread, assistant and RAG files from the OpenAI.</font>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_07_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>08. Add a file to the discussion: </summary>

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
<summary><font size=5>ver 2.2.0</font></summary>
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
<summary>06. Save a discussion: <font color="red">New feature is available.</font></summary>

To Save a log in a discussion is available with the pencil icon `JSON Export`. It will be created a new JSON file as an `opening file + .json` for the Azure OpenAI, and also `opening file + .{model name}.openai.json` that has a threadId and assistantId for the OpenAI.  <font color="red">For the GPT4ALL, `opening file + .{model name}.gpt4all.json`.</font> They will be imported automatically when an original closed file is opened.
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_11_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>07. Delete a discussion: </summary></summary>

To delete a discussion, the cross icon `del thread` is available.
<font color="red">NOTE: It is removed from a JSON file, and also deleting the thread, assistant and RAG files from the OpenAI.</font>
<p align="center">
    <img src="https://github.com/akudo7/kudos-gpt/raw/HEAD/kudos-gpt_07_1.png" />
</p>
</details>
&nbsp;
<details>
<summary>08. Add a file to the discussion: </summary>

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
<summary><font size=5>ver 2.1.0</font></summary>
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

# Comming features soon(I hope...)

- Auto development like OpenDevin
- Publish sample Flowise applications
- Supporting to trained on permissive data with local models

## **Hand-crafted by [Akira Kudo](https://www.linkedin.com/in/akira-kudo-4b04163/) in Tokyo, Japan**

<p align="center">Copyright and Reversed &copy; 2023-present Akira Kudo</p>
