# ChatXporter — AI Chat Conversation Export Tool
ChatXporter is a simple, free, and privacy-focused Chrome extension that allows you to export AI conversations from ChatGPT, Claude, and Gemini into professional formats instantly. All processing happens locally in your browser—your data never leaves your machine.
## 🚀 Features
- 8 Export Formats: Save your chats as PDF, JSON, HTML, HTML (Raw), Markdown, DOCX, TXT, or XML.
- Multi-Platform Support: Seamlessly works with ChatGPT, Claude, and Google Gemini.
- RTL Language Support: Proper handling of Hebrew, Arabic, and other right-to-left languages.
- Customizable UI: Drag and drop the export formats to reorder them based on your preference.
- Theme Aware: Automatically adapts to light or dark mode based on the platform's theme.
- 100% Free: No tiers, no accounts, and no restrictions.
- Privacy-Focused: All processing happens locally; no data is sent to external servers.
## 🛠 Installation
### Developer Mode (Manual Installation)
Currently, the extension can be installed manually using these steps:
1. Download/Clone this repository to your local machine.
2. Open Google Chrome and navigate to `chrome://extensions/`.
3. Enable Developer mode using the toggle in the top-right corner.
4. Click the Load unpacked button.
5. Select the `ai-chat-exporter` folder (the one containing `manifest.json`).
6. The ChatXporter icon should now appear in your toolbar.
## 📖 How to Use
1. Navigate to a supported platform:ChatGPT: https://chatgpt.com or https://chat.openai.comClaude: https://claude.aiGemini: https://gemini.google.com
2. ChatGPT: https://chatgpt.com or https://chat.openai.com
3. Claude: https://claude.ai
4. Gemini: https://gemini.google.com
5. Locate Export Button: Hover your mouse over any AI response.
6. Choose Format: A download icon will appear on the right side of the message; click it to open the menu.
7. Download: Select your desired format to download the file immediately.
## 🔒 Privacy & Permissions
### Privacy Policy
ChatXporter is built with a privacy-first approach.
- No Data Collection: The extension does not collect, track, or transmit any user data.
- Local Processing: All file generation and text extraction happen entirely within your browser session.
### Permissions Justification
- `storage`: Used to save your custom drag-and-drop export format preferences.
- `activeTab` & `tabs`: Required to detect supported chat platforms and reload tabs upon installation to ensure functionality.
- Host Permissions: Necessary to inject export controls directly into the chat interfaces of ChatGPT, Claude, and Gemini.
## 🏗 Technical Details
- Manifest V3: Built using the latest Chrome extension standards.
- Sanitization: Uses DOMPurify to ensure all exported HTML content is safe.
- Architecture:`content.js`: Main entry point for platform detection and UI initialization.`export-manager.js`: Handles message extraction and file generation logic.`sites-config.js`: Contains platform-specific selectors for robust message detection.
- `content.js`: Main entry point for platform detection and UI initialization.
- `export-manager.js`: Handles message extraction and file generation logic.
- `sites-config.js`: Contains platform-specific selectors for robust message detection.
## 📄 License
This extension is provided as-is for personal use.
Version: 1.0.0
