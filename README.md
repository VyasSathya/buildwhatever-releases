# BuildWhatever

AI-native game editor. A Godot 4.6.1 fork with a built-in AI assistant that can read, write, and manipulate your entire project.

**[Download Latest Build](../../releases/latest)**

---

## Quick Start

1. Download `buildwhatever.windows.editor.x86_64.exe` from [Releases](../../releases/latest)
2. Run it — no installer needed, single portable exe
3. Create a new project or open an existing Godot project
4. The **AI Chat** dock is in the left panel

## Setting Up AI

The AI features need an API key to work. You have two options:

### Option A: OpenRouter (Recommended — Cloud)

1. Sign up at [openrouter.ai](https://openrouter.ai)
2. Add credits ($5 is plenty to start)
3. Go to [API Keys](https://openrouter.ai/keys) and create a key
4. In BuildWhatever: **Editor > AI Settings > Add Provider**
5. Select **OpenRouter**, paste your key, hit **Test Connection**

Default model: Kimi K2.5 (~$0.002 per message). You can change models in AI Settings.

### Option B: Ollama (Free — Local)

1. Install [Ollama](https://ollama.com)
2. Pull a model: `ollama pull qwen3` (or `llama3`, `deepseek-r1`, etc.)
3. In BuildWhatever: **Editor > AI Settings > Add Provider**
4. Select **Ollama** — it auto-detects at `localhost:11434`

No API key needed. Runs on your GPU. Needs ~8GB VRAM for good models.

## What Can the AI Do?

- Read, write, and edit scripts and scenes
- Add, delete, and modify nodes in your scene tree
- Generate images (via ComfyUI) and audio (via Kokoro TTS)
- Search your project files and codebase
- Semantic asset search (via Gemini embeddings)
- Plan multi-step changes before executing

### Slash Commands

Type these in the chat input:

| Command | Action |
|---------|--------|
| `/clear` | Clear chat history |
| `/plan` | Toggle plan mode (AI plans before acting) |
| `/model` | Show current model |
| `/export` | Save chat session |
| `/import` | Load chat session |
| `/help` | List commands |

### Tips

- Type `@` to mention and reference project files in your message
- Click `+` to attach an image for AI vision
- Toggle `P` button for plan mode (AI confirms before making changes)
- Code blocks have a **copy** button in the header

## System Requirements

- Windows 10/11 (64-bit)
- GPU with Vulkan support
- ~500MB disk space
- Internet connection (for cloud AI) or ~8GB VRAM (for local Ollama)

## About

BuildWhatever is a fork of [Godot Engine](https://godotengine.org) with integrated AI tools for building games, apps, and interactive experiences. All Godot features and GDScript work as expected.
