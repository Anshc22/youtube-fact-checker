# Privacy Policy — YouTube Fact Checker

**Last updated:** July 22, 2026

## 1. Data We Collect

The YouTube Fact Checker extension collects and stores the following data **locally in your browser only**:

| Data Type | Purpose | Storage |
|-----------|---------|---------|
| AI API Key | Authenticate with your chosen AI provider (OpenAI, Google Gemini, or Anthropic Claude) for fact-checking | `chrome.storage.local` |
| Transcripts | YouTube video captions pulled for analysis | `chrome.storage.local` |
| Speaker Tags | Manual or AI-assisted speaker assignments per video | `chrome.storage.local` |
| Fact-Check Results | AI-generated verdicts, explanations, and sources | `chrome.storage.local` |
| Preferences | Selected provider, model, theme, auto-scroll, and alert settings | `chrome.storage.local` |

## 2. How We Store Data

All data is stored exclusively in your browser's **local extension storage** (`chrome.storage.local`).

- **No data is transmitted to our servers.** We do not operate a backend.
- **No data is synced across devices** unless you use Chrome's built-in profile sync (which is outside our control).
- Data persists until you uninstall the extension or clear extension storage via `chrome://extensions` → "Clear data".

## 3. Third-Party Services

The extension communicates directly with the following services **using your own credentials**:

| Service | Data Sent | Purpose |
|---------|-----------|---------|
| **YouTube** (`youtube.com`) | Video ID | Fetch caption tracks for transcript generation |
| **OpenAI** (`api.openai.com`) | Transcript text + your API key | Generate fact-check verdicts |
| **Google AI Studio** (`generativelanguage.googleapis.com`) | Transcript text + your API key | Generate fact-check verdicts |
| **Anthropic** (`api.anthropic.com`) | Transcript text + your API key | Generate fact-check verdicts |

We do not log, intercept, or store API responses on any intermediate server.

## 4. Data Retention & Deletion

- **Retention:** Data remains in your browser until you uninstall the extension or manually clear it.
- **Deletion:** Uninstalling the extension automatically removes all stored data. You can also clear data via Chrome's extension management page without uninstalling.

## 5. Security

- API keys are stored using Chrome's built-in encrypted storage mechanism (OS-level encryption where available).
- API keys are sent only via HTTPS to the respective AI provider's official API endpoints.
- The Gemini API key is transmitted as a URL query parameter (required by Google's API design); all other providers use HTTP headers.

## 6. Children's Privacy

This extension is not intended for use by children under 13. We do not knowingly collect data from children.

## 7. Changes to This Policy

We will update this policy if our data practices change. The "Last updated" date at the top reflects the most recent revision.

## 8. Contact

For questions or concerns about this privacy policy, contact:

**Email:** [your-email@example.com]  
**Extension:** YouTube Fact Checker V4
