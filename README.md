# sp25-santa-clara-county-wiki

## Overview
This wiki is a comprehensive, maintainable knowledge base of key terms, concepts, and processes relevant to the County of Santa Clara’s data infrastructure, AI initiatives, and governance policies. It is designed for non-technical stakeholders, such as in-house counsel, policymakers, and administrators, to ensure clarity in technical decision-making.


## Installation of Wiki
1. Clone the repository: ```git clone https://github.com/adityaseth8/sp25-santa-clara-county-wiki.git```
2. Launch "Run" Windows Command Script. This can be found within the DokuWikiStick folder
3. Open a web browser and go to ```http://localhost:8800/```

## Usage
- Edit and manage pages using DokuWiki's built-in editor.
- Plugins and templates can be added using DokuWiki's built in extension manager.

### Plugins
Plugins are extensions which extend DokuWiki's features without the need for a programmer to manually modify the wiki's source code, saving time and effort. Please note that many of the plugins available for usage are developed and contributed by the community, as DokuWiki is open source. For security guidelines on plugin usage, please refer to [DokuWiki's plugin security recommendations](https://www.dokuwiki.org/security#plugin_security). The full list of available DokuWiki plugins can be viewed here: [DokuWiki Plugins Directory](https://www.dokuwiki.org/plugins).

To install plugins:
1. Click on "Admin" at top right.
2. Click on Extension Manager.
3. Click on the Search and Install tab.
4. Search the specific plugin and click install.

#### Current Theme & Plugins installed:
 - We have opted to stick with the default DokuWiki theme to ensure long term compatibility with all plugins.
 - [Captcha Plugin](https://www.dokuwiki.org/plugin:captcha): Requires users to complete an audio or visual CAPTCHA during login attempts, adding an extra layer of security to prevent bots from gaining edit access to the County Wiki. The administrator can customize the CAPTCHA types, including options like invisible CAPTCHA, fixed questions, math questions, SVG, and more, through the "Configuration Settings."
 - [DW2PDF Plugin](https://www.dokuwiki.org/plugin:dw2pdf): Export 1 or more DokuWiki paged to PDF.

#### Interesting Plugins for Future Installation:
 - [Statistics Plugin](https://www.dokuwiki.org/plugin:statistics): This plugin allows the wiki administrators to track the wiki traffic, such as the number of views of each page, number of visitors, average session length, etc. Administrators could use this information to determine what aspects of the wiki to better develop, etc. User needs. Our Paragon team has opted not to implement this plugin yet because it requires a MySQL database. We believe it would be best for the County of Santa Clara to implement this plugin using a MySQL database in the County's own private Azure environment.
 - [AI Chat Plugin](https://www.dokuwiki.org/plugin:aichat): This plugin allows users to chat with an LLM of the admin's choice regarding the content on the wiki. The chatbot has the context of whatever content is on the wiki pages so that the chatbot responses to user questions are tailored to that context. The County can experiment with different types of API keys for the LLM, such as OpenAI, Google Gemini, Groq, and more. We recommend exploring using local LLM models like Ollama 3.7 8b because local LLMs provide complete control over data flow and storage, significantly reducing the risk of external breaches.
 - [DeepL Autotranslate Plugin](https://www.dokuwiki.org/plugin:deeplautotranslate): This plugin uses the DeepL API to automatically translate a wiki page to another language, improving accessibility for public wiki viewers. Using DeepL may cost some money.

### General Maintenance
#### Access Control Lists (ACL)
Wiki administrators can restrict access to certain pages using the ACL. This feature can help configure the wiki so that pages containing sensitive internal county information are restricted to county employees, while general pages remain accessible to the public. Full details for ACLs can be viewed [here](https://www.dokuwiki.org/acl).

#### Wiki Hosting Platform
We recommend the County of Santa Clara host this wiki on Azure or any other internal county resource.

#### Resources
[Security Notes](https://www.dokuwiki.org/security)
