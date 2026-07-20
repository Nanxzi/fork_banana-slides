[//]: # "Banana Slides is an AI-native PPT generation app for creating editable presentations from ideas, outlines, documents, images, and custom templates. Features: prompt-to-slide generation, template control, material parsing, conversational editing, PPTX export, project history, and reproducible workflows. Quick Start / Install / Usage / Demo / API / Deploy / Architecture / Test / Screenshot guides are provided for local Docker deployment and online use."
<div align="center">

<p>
  <img src="https://github.com/user-attachments/assets/81fe6816-44cc-4c61-97c7-f3c099650966" alt="Banana Slides" width="860">
</p>
<p>
  <a href="https://trendshift.io/repositories/22056" target="_blank">
    <img src="https://trendshift.io/api/badge/repositories/22056" alt="Anionex%2Fbanana-slides | Trendshift" width="265" height="58">
  </a>
  <br>
  <a href="https://hellogithub.com/repository/Anionex/banana-slides" target="_blank">
    <img src="https://abroad.hellogithub.com/v1/widgets/recommend.svg?rid=c8a0ee51918e4353af08012b8472b85e&claim_uid=CtDTm2jbUHhVGBr&theme=neutral" alt="Featured｜HelloGitHub" width="265" height="58">
  </a>
</p>
<p>
  <a href="#-项目缘起"><b>简体中文</b></a>
  &nbsp;•&nbsp;
  <a href="README_EN.md"><b>English</b></a>
</p>
<p>
  <a href="https://github.com/Anionex/banana-slides/stargazers"><img src="https://img.shields.io/github/stars/Anionex/banana-slides?style=flat-square&color=FFD700" alt="GitHub Stars"></a>
  <a href="https://github.com/Anionex/banana-slides/network"><img src="https://img.shields.io/github/forks/Anionex/banana-slides?style=flat-square&color=FFD700" alt="GitHub Forks"></a>
  <a href="https://github.com/Anionex/banana-slides/watchers"><img src="https://img.shields.io/github/watchers/Anionex/banana-slides?style=flat-square&color=FFD700" alt="GitHub Watchers"></a>
  <a href="https://github.com/Anionex/banana-slides/releases/tag/v0.9.0-rc.2"><img src="https://img.shields.io/badge/version-v0.9.0--rc.2-44cc11?style=flat-square" alt="Version"></a>
  <a href="https://github.com/Anionex/banana-slides/blob/main/LICENSE"><img src="https://img.shields.io/github/license/Anionex/banana-slides?color=0055aa&style=flat-square" alt="License"></a>
  <br>
  <img src="https://img.shields.io/badge/Docker-Build-4A90D9?logo=docker&logoColor=white&style=flat-square" alt="Docker Build">
  <a href="https://deepwiki.com/Anionex/banana-slides"><img src="./assets/badge-deepwiki-flat.svg" alt="Ask DeepWiki"></a>
</p>

<p>
  <b>An AI-native PPT generation application based on nano banana pro 🍌</b><br>
  <b>Go from ideas to presentations in minutes—no tedious formatting, request edits conversationally, and move towards true "Vibe PPT"</b>
</p>
<p>
  <a href="https://bananaslides.online/"><b>🚀 Online Demo</b></a>
  &nbsp;|&nbsp;
  <a href="https://docs.bananaslides.online/"><b>📖 Documentation</b></a>
  &nbsp;|&nbsp;
  <a href="https://github.com/Anionex/banana-slides/releases/tag/v0.9.0-rc.2"><b>💻 Desktop RC2</b></a>
  &nbsp;|&nbsp;
 <a href="https://github.com/Anionex/banana-slides#-%E4%BD%BF%E7%94%A8%E6%96%B9%E6%B3%95"><b>Deployment</b></a>
</p>
<p>
  If this project is helpful to you, please give it a <b>Star 🌟</b> & <b>Fork 🍴</b>
</p>

</div>

## 🔥 Latest Updates

- **[2026-07-15]**: Custom outline/description requirement presets now automatically repair corrupted browser cache, preserving valid presets and preventing abnormal cache from blocking the editor page.
- **[2026-07-11]**: 0.9.0 Release Candidate 2 is out, including all capabilities of RC1 while fixing MinerU directory inconsistencies for editable PPTX on Windows desktop and FFprobe path errors for instructional videos; [One-click download and install](https://github.com/Anionex/banana-slides/releases/tag/v0.9.0-rc.2)
- **[2026-06-23]**: Page-by-page templates launched — Supports both single and multi-template modes. Upload images or PDFs to build project template libraries; AI automatically parses template styles and intelligently matches them to each page with one click, or bind them manually per page. Supports seamless bidirectional switching between modes ([Docs](https://docs.bananaslides.online/zh/features/templates))
- **[2026-04-25]**: Asset Toolbox launched — Adds three new modes to the existing asset generation: full-image editing, marquee editing (overlay/replace), and smart erase, providing a unified one-stop entry for operations.
- **[2026-04-25]**: Supports account binding via official OpenAI OAuth. Once bound, Codex can be used directly as the text/image generation provider without manually entering an API Key. Plus accounts can generate 100+ 2K images every five hours ([Tutorial](https://ziy68cvfvu3.feishu.cn/wiki/LDSOwPzkhiNonkkNTF1ct2VBnNc)) (Based on official OpenAI OAuth PKCE authorization flow, not reverse engineered).
- **[2026-04-25]**: Supports saving custom text style description templates. You can name, color-code, and persistently reuse them without re-entering every time.
- **[2026-04-23]**: Added support for the gpt-image-2 model. Meanwhile, editable background effects have been improved due to model upgrades (Select "Generative Retrieval" in Settings - Export Options - Background Retrieval).
- **[2026-04-11]**: Added support for [CLI operations and integrated agent skills](https://docs.bananaslides.online/cli).
- **[2026-03]**: Added several features and optimizations, such as extra fields and multi-aspect ratio settings.
- **[2026-02-09]**: New features and optimizations
  * New Features
    * Supports pasting images on the home page, outline, and description cards for immediate recognition, with an improved interaction experience.
    * Manual outline section editing: Supports manual adjustment of the section (part) a page belongs to.
    * Docker Multi-arch: Images now support amd64 / arm64 builds.
    * Internationalization + Dark Mode: Added Chinese/English switching; supports Light/Dark/Follow System themes; all components adapted for dark mode.
  * Fixes & UX Optimizations
    * Fixed export-related 500 errors, reference file association timing, outline/page data misalignment, incorrect task polling items, infinite polling for description generation, image preview memory leaks, and partial failures in batch deletions.
    * Optimized format example hints, HTTP error message copy, Modal closing experience, cleanup of old project localStorage, and removed redundant prompts for first-time project creation.
    * Various other optimizations and fixes.

> **Desktop Version Configuration, Storage, and Export Tips**: The desktop installer does not have a `.env` file in the project root; please save API configurations directly in "Settings". Upon first installation on Windows, you can choose the "Data Storage Location"; all desktop platforms can also change this in "Settings → Data Storage Location" (takes effect after restart). The app does not automatically migrate or delete old data; before manual migration, you must fully exit the app from the tray and copy the `data`, `uploads`, and `exports` directories in full. The desktop version completes OpenAI OAuth in the system browser and automatically shows as connected upon success without needing to refresh the app. Desktop exports will trigger a system save dialog and are only considered complete once the file is successfully written to the chosen location; if writing fails, the target path and error message will be shown, or you can redownload from the "Export Tasks" panel.

## ✨ Project Origin

Have you ever found yourself in this dilemma: a presentation is due tomorrow, but your PPT is still a blank slate; your mind is brimming with brilliant ideas, yet your enthusiasm is drained by the tediousness of layout and design?

We long to quickly create presentations that are both professional and well-designed. While traditional AI PPT generation apps generally meet the need for "speed," they still suffer from the following issues:

- 1️⃣ Limited to preset templates with no flexibility to adjust styles
- 2️⃣ Low degree of freedom, making multi-round revisions difficult
- 3️⃣ Similar visual output resulting in severe homogenization
- 4️⃣ Low-quality assets that lack specificity
- 5️⃣ Disconnected image and text layouts with a poor sense of design

These deficiencies make it difficult for traditional AI PPT generators to simultaneously satisfy our two core requirements: "speed" and "aesthetics." Even those claiming to be "Vibe PPT" are, in my view, far from truly having that "Vibe."

However, the emergence of the **nano banana 🍌** model has changed everything. I experimented with **🍌pro** for PPT page generation and found that the results—in terms of quality, aesthetics, and consistency—were outstanding. It can almost precisely render all text requested by the prompt while strictly adhering to the style of reference images. So, why not build a native "Vibe PPT" application based on **🍌pro**?

## 👨‍💻 Use Cases

1. **Beginners**: Generate beautiful PPTs quickly with zero barrier to entry, no design experience required, reducing the hassle of template selection.
2. **PPT Professionals**: Reference AI-generated layouts and text-image combinations to quickly gain design inspiration.
3. **Educators**: Quickly convert teaching content into illustrated lesson plan PPTs to enhance classroom effectiveness.
4. **Students**: Complete class presentations quickly, focusing energy on content rather than layout and design.
5. **Workplace Professionals**: Quickly visualize business proposals and product introductions with fast adaptation across multiple scenarios.

<p>
  <b>🎯Goal: Lower the barrier to PPT creation, enabling everyone to quickly produce beautiful and professional presentations.</b>
</p>

## 🎨 Result Examples

<div align="center">

| | |
|:---:|:---:|
| <img src="https://github.com/user-attachments/assets/d58ce3f7-bcec-451d-a3b9-ca3c16223644" width="500" alt="Case 3"> | <img src="https://github.com/user-attachments/assets/c64cd952-2cdf-4a92-8c34-0322cbf3de4e" width="500" alt="Case 2"> |
| **Software Development Best Practices** | **DeepSeek-V3.2 Technical Showcase** |
| <img src="https://github.com/user-attachments/assets/383eb011-a167-4343-99eb-e1d0568830c7" width="500" alt="Case 4"> | <img src="https://github.com/user-attachments/assets/1a63afc9-ad05-4755-8480-fc4aa64987f1" width="500" alt="Case 1"> |
| **R&D and Industrialization of Intelligent Production Equipment for Prepared Meals** | **The Evolution of Money: From Shells to Banknotes** |

</div>

See more at <a href="https://github.com/Anionex/banana-slides/issues/2" > Use Cases </a>

## 🎯 Features

### 1. Flexible and Diverse Creation Paths

Supports three starting modes: **Idea**, **Outline**, and **Page Description**, catering to different creative workflows.
- **One-Sentence Generation**: Enter a topic, and the AI automatically generates a well-structured outline and page-by-page content descriptions.
- **Natural Language Editing**: Supports modifying outlines or descriptions via "Vibe" prompts (e.g., "Change page three to a case study"), with the AI responding and adjusting in real-time.
- **Outline/Description Mode**: Supports both one-click batch generation and manual fine-tuning of details.
- **Reliable Markdown Import**: The import dialog previews the number of recognized pages before execution and appends pages sequentially according to the file order, preventing formatting errors or unpredictable page sequences after multi-page imports.

<img width="2000" height="1125" alt="image" src="https://github.com/user-attachments/assets/7fc1ecc6-433d-4157-b4ca-95fcebac66ba" />

### 2. Powerful Asset Parsing Capabilities

- **Multi-format Support**: Upload PDF, Docx, MD, Txt, and other files for automatic background content parsing.
- **Intelligent Extraction**: Automatically identify key points, image links, and chart information within the text to provide rich materials for generation.
- **Automatic Image Storage**: Images extracted from documents will automatically enter the project material library after the reference file is associated with the project, allowing for direct reuse in the future.
- **Style Reference**: Support uploading reference images or templates to customize the PPT style.
- **Multi-image Joint Reference**: When using GPT Image, the image templates and material images in the page description are passed to the model together, rather than only using the first reference image.

<img width="1920" height="1080" alt="Document Parsing and Material Processing" src="https://github.com/user-attachments/assets/8cda1fd2-2369-4028-b310-ea6604183936" />

### 3. "Vibe"-style natural language modification

No longer restricted by complex menu buttons; issue modification commands directly using **natural language**.
- **Inpainting**: Make conversational modifications to specific areas (e.g., "Change this chart to a pie chart").
- **Full-Page Optimization**: Generate high-definition, stylistically consistent pages powered by nano banana pro🍌.
- **Quality Control Mode**: Can be enabled in system settings or the preview page; automatically checks for garbled text, low-quality visuals, and prompt deviation after generation. Only images that pass the check are saved as new versions.

<img width="2000" height="1125" alt="image" src="https://github.com/user-attachments/assets/929ba24a-996c-4f6d-9ec6-818be6b08ea3" />

### 4. Out-of-the-Box Format Export

- **Multi-format Support**: One-click export to standard **PPTX** or **PDF** files.
- **Playback Settings**: Enable slide transition animations before exporting PPTX. Supports classic effects such as Fade, Flip, Pan, Wipe, Split, Blinds, Checkerboard, and Clock, with support for random application from multiple selections.
- **Exported File Management**: The preview page lists files already exported on the server, allowing you to download them directly or delete unnecessary files. Export task history is isolated by project to prevent accidental deletion of records from other projects. If a backend task is no longer available after a refresh, the task panel clearly displays a failure status and prompts for re-export.
- **Video Export Configuration Pre-check**: Displays the loading state for settings before opening the narration video panel. If the output language or ElevenLabs configuration fails to load, a clear prompt to retry is shown instead of proceeding with uncertain default values.
- **Clearer Selective Page Export**: The selective page export now indicates missing images based on the currently selected range. Unselected draft pages will no longer disable the export entry for selected completed pages. Narration videos will only include pages without images if the placeholder frame option is explicitly checked.
- **Perfect Fit**: Default 16:9 ratio; no secondary layout adjustments required, ready for direct presentation.

<img width="1000" alt="image" src="https://github.com/user-attachments/assets/3e54bbba-88be-4f69-90a1-02e875c25420" />
<img width="1748" height="538" alt="PPT与PDF导出" src="https://github.com/user-attachments/assets/647eb9b1-d0b6-42cb-a898-378ebe06c984" />

### 5. Fully Editable PPTX Export (Beta)

- **Export images as high-fidelity, clean-background PPT pages with freely editable images and text**
- For related updates, see https://github.com/Anionex/banana-slides/issues/121
<img width="1000"  alt="image" src="https://github.com/user-attachments/assets/a85d2d48-1966-4800-a4bf-73d17f914062" />

### 6. One-click Export of Explainer Videos

- **One-click conversion of slides into presentation videos (MP4) with AI voiceover and subtitles**
- AI automatically generates spoken-style narrations based on page descriptions and content
- Supports configuration of various expression styles, multiple languages, and diverse voice tones

<br>

**🌟 Comparison with NotebookLM Slide Deck Features**
| Feature | NotebookLM | This Project | 
| --- | --- | --- |
| Page Limit | 15 pages | **Unlimited** | 
| Re-editing | Prompt-based modification | **Selection-based editing + Verbal editing** |
| Asset Addition | Cannot add after generation | **Add freely after generation** |
| Export Formats | Supports PDF, (non-editable image) PPTX | **Export to PDF, (image or editable) PPTX, Presentation Video** |
| Watermark | Watermark in free version | **No watermark, freely add/remove elements** |

> Note: This comparison may become outdated as new features are added.

## 🗺️ Roadmap

| Status | Milestones |
| --- | --- |
| ✅ Completed | Create PPTs via three paths: ideas, outlines, and page descriptions |
| ✅ Completed | Parse Markdown format images in text |
| ✅ Completed | Add more assets to a single PPT page |
| ✅ Completed | Vibe voice editing for selected areas on a single PPT page |
| ✅ Completed | Asset module: Asset generation, uploading, etc. |
| ✅ Completed | Support for uploading and parsing multiple file types |
| ✅ Completed | Support Vibe voice adjustments for outlines and descriptions |
| ✅ Completed | Initial support for exporting editable .pptx files |
| 🔄 In Progress | Support multi-layered, precise cutout editable .pptx export |
| 🔄 In Progress | Web search |
| 🔄 In Progress | Agent mode |
| ✅ Completed | TTS narration video export (CN/EN/JP multi-voice, subtitles) |
| 🚍 Partial | Optimize frontend loading speed |
| 🧭 Planned | Online playback feature |
| 🧭 Planned | Simple animations and page transition effects |
| 🚍 Partial | Multi-language support |
| | |

## 📦 Usage

### (New) One-click Deployment Using Application Templates

This is the simplest way, with no need to install Docker or download the project. You can access the application directly after creation.


1. One-click deploy and launch this application via Rainyun (High bandwidth, ideal for HD image generation and downloading. Free trials available for new users)
- [Graphic Tutorial](https://ziy68cvfvu3.feishu.cn/wiki/B5RIwg3OUiCfo9kyadzcR9CInnc?from=from_copylink)

[![通过雨云一键部署](https://rainyun-apps.cn-nb1.rains3.com/materials/deploy-on-rainyun-cn.svg)](https://app.rainyun.com/apps/rca/store/7549/anionex_)

2. Coming soon

### Using Docker Compose🐳

Quickly start front-end and back-end services via Docker Compose.

<details>
  <summary>📒 Instructions for Windows/Mac Users</summary>

If you are using **Windows or macOS**, please [install **Docker Desktop**](https://docs.docker.com/desktop/setup/install/windows-install/) first and ensure that Docker is running (check the system tray icon on Windows or the menu bar icon on macOS), then follow the same steps in the documentation.

> **Tip**: If you encounter any issues, Windows users should enable the **WSL 2 backend** in Docker Desktop settings (recommended); also, ensure that ports **3011** and **5011** are not occupied.

</details>

0. **Clone the repository**
```bash
git clone https://github.com/Anionex/banana-slides
cd banana-slides
```

1. **Configure environment variables**

Create a `.env` file (refer to `.env.example`):
```bash
cp .env.example .env
```

**(Optional: You can also configure via the user interface after startup. [Click here for the tutorial](https://ziy68cvfvu3.feishu.cn/wiki/GiNawdmpiinSRqkGspocqEWAnkh?from=from_copylink))** Edit the `.env` file and configure the necessary environment variables:

<details>
<summary>Click to expand details</summary>
  
> **The LLM interfaces in this project follow the AIHubMix platform format. It is recommended to use [AIHubMix (click here to access directly)](https://api.inferera.com/?aff=17EC) to obtain API keys to reduce migration costs.**<br>
> **Friendly Reminder: The API costs for the Google nano banana pro model are relatively high; please be mindful of usage costs.**
```env

# AI Provider Format Configuration (gemini / openai / volcengine / vertex)

AI_PROVIDER_FORMAT=gemini

# Gemini Format Configuration (Used when AI_PROVIDER_FORMAT=gemini)

GOOGLE_API_KEY=your-api-key-here
GOOGLE_API_BASE=https://generativelanguage.googleapis.com

# Proxy Example: https://api.inferera.com/gemini

# OpenAI Format Configuration (Used when AI_PROVIDER_FORMAT=openai)

OPENAI_API_KEY=your-api-key-here
OPENAI_API_BASE=https://api.openai.com/v1

# Proxy Example: https://api.inferera.com/v1

# Volcengine Ark AgentPlans Configuration (Used when AI_PROVIDER_FORMAT=volcengine)

VOLCENGINE_API_KEY=your-volcengine-api-key-here
VOLCENGINE_API_BASE=https://ark.cn-beijing.volces.com/api/v3

# Vertex AI Configuration (AI_PROVIDER_FORMAT=vertex)

# GCP Project and Service Account Key Required

# VERTEX_PROJECT_ID=your-gcp-project-id

# VERTEX_LOCATION=global

# GOOGLE_APPLICATION_CREDENTIALS=./gcp-service-account.json

# Lazyllm Format Configuration (Used when AI_PROVIDER_FORMAT=lazyllm)

# Selecting Providers for Text and Image Generation

TEXT_MODEL_SOURCE=deepseek        # Text generation model provider
IMAGE_MODEL_SOURCE=doubao         # Image editing model provider
IMAGE_CAPTION_MODEL_SOURCE=qwen   # Image captioning model provider

# API Keys for Various Providers (Only configure those you intend to use)

```env
DOUBAO_API_KEY=your-doubao-api-key            # Volcengine/Doubao
DEEPSEEK_API_KEY=your-deepseek-api-key        # DeepSeek
QWEN_API_KEY=your-qwen-api-key                # Alibaba Cloud/Qwen
GLM_API_KEY=your-glm-api-key                  # Zhipu GLM
SILICONFLOW_API_KEY=your-siliconflow-api-key  # SiliconFlow
SENSENOVA_API_KEY=your-sensenova-api-key      # SenseTime SenseNova
MINIMAX_API_KEY=your-minimax-api-key          # MiniMax
...
```

> Banana Slides explicitly packages the LazyLLM online provider SDKs used by Chinese providers:
> `volcengine-python-sdk[ark]` for Doubao, `dashscope` for Qwen/Wanxiang, and `zhipuai` for GLM/Zhipu.
> LazyLLM also exposes `lazyllm install online-advanced`, but the PyPI wheel may not publish that group as a standard install extra, so Docker/prebuilt images rely on these explicit dependencies instead.
  
</details>


**Use the new editable export configuration method to achieve better editable export results**: You need to obtain an API KEY from the [Baidu AI Cloud Platform](https://console.bce.baidu.com/iam/#/iam/apikey/list) (click here to enter) and fill it in the `BAIDU_API_KEY` field of the `.env` file (sufficient free usage quota available). For details, please refer to the instructions in https://github.com/Anionex/banana-slides/issues/121


<details>
  <summary>📒 Vertex AI Configuration Guide (for GCP Users)</summary>

Google Cloud Vertex AI allows calling Gemini models via GCP service accounts; new users can use free trial credits. Configuration steps:

1. Go to the [GCP Console](https://console.cloud.google.com/), create a service account, and download the JSON key file.
2. Save the key file as `gcp-service-account.json` in the project root directory.
3. Set in `.env`:
   ```env
   AI_PROVIDER_FORMAT=vertex
   VERTEX_PROJECT_ID=your-gcp-project-id
   VERTEX_LOCATION=global
   ```
4. If deploying with Docker, you also need to uncomment the relevant sections in `docker-compose.yml`, mount the key file into the container, and set the `GOOGLE_APPLICATION_CREDENTIALS` environment variable.

> The `gemini-3-*` series models require `VERTEX_LOCATION=global`

</details>

2. **Start the Service**

**⚡ Using Pre-built Images (Recommended)**

The project provides pre-built frontend and backend images on Docker Hub (synchronized with the latest version of the main branch), allowing you to skip local build steps and achieve rapid deployment:

```bash

# Start with Pre-built Images (No need to build from scratch)

docker compose -f docker-compose.prod.yml up -d
```

Image Names:
- `anoinex/banana-slides-frontend:latest`
- `anoinex/banana-slides-backend:latest`

After startup, you can navigate to **Settings → About → Check for Updates** within the application. The app will determine if an update is available based on the current version SHA; when running from source, the current Git SHA will also be used for this check.

**Build Images from Scratch**

```bash
docker compose up -d
```


> [!TIP]
> If you encounter network issues, you can uncomment the mirror source configuration in the `.env` file and then rerun the startup command:
> ```env
> # Uncomment the following lines in the .env file to use domestic mirror sources in China
> DOCKER_REGISTRY=docker.1ms.run/
> GHCR_REGISTRY=ghcr.nju.edu.cn/
> APT_MIRROR=mirrors.aliyun.com
> PYPI_INDEX_URL=https://mirrors.cloud.tencent.com/pypi/simple
> NPM_REGISTRY=https://registry.npmmirror.com/
> ```


3. **Access the Application**

- Frontend: http://localhost:3011
- Backend API: http://localhost:5011

4. **View Logs**

```bash

# View Backend Logs (Last 200 Lines)

docker logs --tail 200 banana-slides-backend

# View Backend Logs in Real-time (Last 100 Lines)

docker logs -f --tail 100 banana-slides-backend

# View Frontend Logs (Last 100 Lines)

docker logs --tail 100 banana-slides-frontend
```

5. **Stop Services**

```bash
docker compose down
```

6. **Update Project**

**Using Pre-built Images (docker-compose.prod.yml)**

You can also go to **Settings → About → Check for Updates** within the app first to see if a new version is available.

```bash
docker compose -f docker-compose.prod.yml pull
docker compose -f docker-compose.prod.yml up -d
```

**Using Local Build (docker-compose.yml)**

Note: If you have manually modified the code, this method is not applicable. You need to revert the code to the version at the time of the pull first.

```bash
git pull 
docker compose down
docker compose build --no-cache
docker compose up -d
```

**Note: Thanks to our excellent developer friend [@ShellMonster](https://github.com/ShellMonster/) for providing the [Newbie Deployment Tutorial](https://github.com/ShellMonster/banana-slides/blob/docs-deploy-tutorial/docs/NEWBIE_DEPLOYMENT.md). It is specifically designed for beginners without any server deployment experience. You can [click the link](https://github.com/ShellMonster/banana-slides/blob/docs-deploy-tutorial/docs/NEWBIE_DEPLOYMENT.md) to view it.**

### Deploy from Source

#### Environment Requirements

- Python 3.10 or higher
- [uv](https://github.com/astral-sh/uv) - Python package manager
- Node.js 16+ and npm
- [FFmpeg](https://ffmpeg.org/) - Required for exporting explanation videos; must include `libass` / `ass` subtitle filter support
- A valid Google Gemini API key
- (Optional) [LibreOffice](https://www.libreoffice.org/) - Required when uploading PPTX files using the "PPT Refurbishment" feature, used to convert PPTX to PDF. **It is recommended to convert PPTX to PDF locally before uploading**. Reason: Server-side rendering with LibreOffice may cause layout misalignment due to missing fonts (such as Microsoft YaHei, Calibri, etc.) and cannot fully restore some special effects. LibreOffice is not required if you upload PDF files. Docker users who still need PPTX upload support within the container can execute:
  ```bash
  docker exec -it banana-slides-backend bash -c "apt-get update && apt-get install -y libreoffice-impress && rm -rf /var/lib/apt/lists/*"
  ```
  > Note: LibreOffice installed this way will be lost after the container is rebuilt and must be reinstalled.

#### Backend Installation

0. **Clone the repository**
```bash
git clone https://github.com/Anionex/banana-slides
cd banana-slides
```

1. **Install uv (if not already installed)**
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

2. **Install dependencies**

Run in the project root directory:
```bash

# macOS (Homebrew)

brew install ffmpeg-full
brew unlink ffmpeg 2>/dev/null || true
brew link --overwrite --force ffmpeg-full

# Ubuntu / Debian

```bash
sudo apt-get update
sudo apt-get install -y ffmpeg libass9
```

# Then install Python dependencies

uv sync
```

This will automatically install all dependencies based on `pyproject.toml`.

3. **Configure Environment Variables**

Copy the environment variable template:
```bash
cp .env.example .env
```

# Then, follow the previously mentioned method to open and edit the `.env` file and configure your API key

It appears that you haven't provided any Chinese Markdown content in the "Original content" section. Please paste the text you would like me to translate, and I will be happy to follow your requirements!

#### Frontend Installation

1. **Enter the frontend directory**
```bash
cd frontend
```

2. **Install dependencies**
```bash
npm install
```

3. **Configure API address**

The frontend will automatically connect to the backend service specified by `BACKEND_PORT` (default `http://localhost:5011`) via Vite proxy. To modify this, please set `BACKEND_PORT` in the `.env` file at the project root.

#### Start Backend Service

> (Optional) If you have important local data, it is recommended to back up the database before upgrading:  
> `cp backend/instance/database.db backend/instance/database.db.bak`
> Note: Under default configuration, templates, assets, and final products are all stored in the `uploads/` folder.

```bash
cd backend
uv run alembic upgrade head && uv run python app.py
```

The backend service will start at `http://localhost:5011`.

Visit `http://localhost:5011/health` to verify that the service is running correctly.

#### Start Front-end Development Server

```bash
cd frontend
npm run dev
```

The frontend development server will start at `http://localhost:3011`.

Open your browser and visit the address to use the application.

## 🛠️ Technical Architecture

### Frontend Technology Stack

React 18 + TypeScript + Vite 5 + Zustand

### Backend Tech Stack

Python 3.10+ + Flask 3.0 + uv + SQLite

## Communication Group

New feature suggestions and feedback are welcome, and I will also answer questions in a ~~laid-back~~ manner.

<img width="312" alt="image" src="https://github.com/user-attachments/assets/aa7756f3-18d5-456f-9f2e-6a541fb1c444" />

Feel free to follow the author's social media, where I will share information about this project and AI:

<p>
  <a href="https://x.com/anion_ex"><img src="https://img.shields.io/badge/X-@anion__ex-000000?style=flat-square&logo=x&logoColor=white" alt="X (Twitter)"></a>
  <a href="https://www.xiaohongshu.com/user/profile/62e8f580000000001902fc9d"><img src="https://img.shields.io/badge/小红书-Anion-FF2442?style=flat-square&logo=xiaohongshu&logoColor=white" alt="Xiaohongshu"></a>
  <a href="https://space.bilibili.com/477162339"><img src="https://img.shields.io/badge/Bilibili-Anion-00A1D6?style=flat-square&logo=bilibili&logoColor=white" alt="Bilibili"></a>
</p>

## **🔧 Frequently Asked Questions**

Refer to the [official documentation](https://docs.bananaslides.online/zh/faq)

You can also ask questions directly on DeepWiki 
<a href="https://deepwiki.com/Anionex/banana-slides"><img src="https://deepwiki.com/badge.svg" alt="Ask DeepWiki"></a>

## 🤝 Contributing Guide

Welcome to contribute to this project via
[Issue](https://github.com/Anionex/banana-slides/issues)
and
[Pull Request](https://github.com/Anionex/banana-slides/pulls)!

> **Important:** Please read [CONTRIBUTING.md](CONTRIBUTING.md) before contributing

## 📄 License

This project is open-sourced under the **GNU Affero General Public License v3.0 (AGPL-3.0)**. It can be freely used for non-commercial purposes such as personal study, research, testing, education, or non-profit scientific research;

For inquiries or potential collaboration, please contact: davidyang042@gmail.com

<h2>🚀 Sponsor</h2>
<br>
<div align="center">
<a href="https://api.inferera.com/?aff=17EC">
  <img src="./assets/logo_aihubmix.png" alt="AIHubMix" style="height:48px;">
</a>
<p>Thanks to AIHubMix for sponsoring this project</p>
</div>

<div align="center">
<a href="英文链接">
    <img src="./assets/byteplus.png" alt="BytePlus" width="150"/ >
    <p> Thanks to BytePlus for sponsoring this project! Register via <a href="https://www.byteplus.com/en/product/modelark?utm_campaign=hw&utm_content=banana-slides&utm_medium=devrel_tool_web&utm_source=OWO&utm_term=banana-slides">this link</a> to get 500,000 tokens of free inference quota per model. </p>
</a>
</div>

<div align="center">

 <br>

<a href="https://api.chatfire.site/login?inviteCode=A15CD6A0"><img width="200" alt="image" src="https://github.com/user-attachments/assets/d6bd255f-ba2c-4ea3-bd90-fef292fc3397" />
</a>

Thanks to ChatFire for sponsoring this project
 
</div>

## Acknowledgements

- Project contributors:

[![Contributors](https://contrib.rocks/image?repo=Anionex/banana-slides)](https://github.com/Anionex/banana-slides/graphs/contributors)

- [Linux.do](https://linux.do/): A new ideal community

## Appreciation

Open source is not easy 🙏 If this project is valuable to you, feel free to buy the developer a coffee ☕️

<img width="240" alt="image" src="https://github.com/user-attachments/assets/fd7a286d-711b-445e-aecf-43e3fe356473" />

Thanks to the following friends for their voluntary sponsorship and support of the project:
> @雅俗共赏、@曹峥、@以年观日、@John、@胡yun星Ethan, @azazo1、@刘聪NLP、@🍟、@苍何、@万瑾、@biubiu、@law、@方源、@寒松Falcon、@刘星宇&小陀螺AIGC
> If you have any questions regarding the sponsorship list, please <a href="mailto:davidyang042@gmail.com">contact the author</a>

## 📈 Project Statistics

<a href="https://www.star-history.com/#Anionex/banana-slides&type=Timeline&legend=top-left">

 <picture>

   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Anionex/banana-slides&type=Timeline&theme=dark&legend=top-left" />

   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=Anionex/banana-slides&type=Timeline&legend=top-left" />

   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=Anionex/banana-slides&type=Timeline&legend=top-left" />

 </picture>

</a>

<br>
