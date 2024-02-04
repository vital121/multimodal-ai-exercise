# Multimodal version of a chatbot powered by OpenAI GPT4

I'm enhancing an interactive system that integrates the GPT-4 Vision API with real-time video streaming, enabling users to interact through speech without UI engagement. To represent video streams, This is a new inovational method using a grid of sequential screenshots. This approach required refining system prompts to interpret the grid as a continuous video, focusing on temporal sequence and direct user interactions. The system, developed through iterative improvements and user feedback, leverages spatial-temporal analysis for precise, user-centric responses. Additionally, it utilizes Whisper for voice transcription and text-to-speech conversion. The app is a prototype with areas for improvement, like response speed and complex question handling. It operates in a turn-based interaction mode, with potential for future enhancements.

## ✨ Demo

/////////////////////

You'll need an OpenAI API key. Remember to delete the API key after using it sor safety.

## 🛠 Stack

- Next.js with App Router.
- Vercel AI npm module.
- OpenAI's Whisper and GPT APIs.

## 🚀 Getting Started

You can provide the `OPENAI_API_KEY`` environment variable or let the user provide its own API key in the UI.

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

## 🔧 Constants

Some constants are fixed at the top of `/src/app/page.js`. You may want to tweak these :

```js
const INTERVAL = 250;
const IMAGE_WIDTH = 512;
const IMAGE_QUALITY = 0.6;
const COLUMNS = 4;
const MAX_SCREENSHOTS = 60;
const SILENCE_DURATION = 2500;
const SILENT_THRESHOLD = -30;
```
