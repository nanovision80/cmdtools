# 🚀 Command-Line (CLI) Tools Curation — Expansion

New hand-picked tools to complement the original curation, including category leaders for specific niches as well as emerging alternatives focused on performance and AI.

---

## 🎬 Media Manipulation (Video, Audio and Image)

- **vips (libvips)** (Image Processing): Image processing library and CLI with drastically lower memory usage and higher speed than ImageMagick on large images.
  - *Strength:* Processes huge images (maps, scans, satellite imagery) without blowing up RAM, thanks to streaming/pipeline processing.
  - *Target Audience:* Backend developers processing images at scale or in production.

- **realesrgan-ncnn-vulkan** (Image Processing / AI): Neural-network-based image upscaling tool (Real-ESRGAN), running via CLI with Vulkan acceleration.
  - *Strength:* Upscales image/video frame resolution with quality far superior to traditional interpolation algorithms.
  - *Target Audience:* Video editors, image restorers, and generative AI enthusiasts.

- **oxipng** (Image Optimization): PNG optimizer written in Rust, focused on ultra-fast lossless compression.
  - *Strength:* Multithreaded and significantly faster than the classic `optipng`, while keeping the same compression ratio.
  - *Target Audience:* Web developers and CI/CD pipelines that optimize assets automatically.

- **chafa** (Image Viewing): Renders images and GIFs directly in the terminal using Unicode/ANSI/Sixel characters.
  - *Strength:* Lets you preview images without leaving the command line, with support for modern terminals (Kitty, iTerm2).
  - *Target Audience:* Developers working entirely over SSH/remote terminals.

- **whisper.cpp** (Audio Transcription / AI): Ultra-lightweight C/C++ implementation of OpenAI's Whisper model for offline audio transcription.
  - *Strength:* Runs locally without a dedicated GPU, without sending sensitive data to external APIs.
  - *Target Audience:* Journalists, content creators, and developers who need private, offline transcription.

---

## 🌐 Networking, Downloads and APIs

- **xh** (HTTP Client): HTTPie alternative written in Rust, with compatible syntax but much faster startup performance.
  - *Strength:* Combines HTTPie's usability with Rust's native speed — ideal for scripts making many calls.
  - *Target Audience:* API developers looking for a faster HTTPie.

- **ngrok** (Tunneling & Network Exposure): Creates secure tunnels that expose a local server to the internet instantly.
  - *Strength:* One-command simplicity for testing webhooks and demos without configuring DNS or firewalls.
  - *Target Audience:* Full-stack developers testing external integrations (Stripe, Twilio, etc.).

- **grpcurl** (API Testing): The `curl` equivalent for gRPC services, allowing inspection and invocation of gRPC endpoints.
  - *Strength:* Supports server reflection, eliminating the need for local `.proto` files.
  - *Target Audience:* Backend/microservices engineers working with gRPC.

- **rustscan** (Security/Scanning): Ultra-fast port scanner written in Rust that feeds results directly into Nmap.
  - *Strength:* Scans all 65,535 ports in seconds, much faster than Nmap alone.
  - *Target Audience:* Pentesters and offensive security professionals.

- **doggo** (DNS): Command-line client for DNS queries with colorful, readable output, replacing `dig`.
  - *Strength:* Human-friendly interface and native DoH (DNS over HTTPS) support, something `dig` doesn't offer natively.
  - *Target Audience:* SREs and network administrators.

---

## 📂 Data Handling and Processing

- **miller (mlr)** (Data Processing): "Swiss army knife" for CSV, TSV, and JSON, combining the functions of `awk`, `sed`, `cut`, and `join` into a single format-agnostic tool.
  - *Strength:* Handles heterogeneous tabular data with a unified syntax, without switching between tools.
  - *Target Audience:* Data analysts and engineers doing lightweight ETL via terminal.

- **visidata (vd)** (Data Exploration): Interactive terminal spreadsheet tool for navigating, filtering, and analyzing large tabular datasets.
  - *Strength:* Opens multi-million-row CSVs instantly — something that would choke Excel/Google Sheets.
  - *Target Audience:* Data scientists and analysts exploring raw data quickly.

- **dasel** (Data Selector): Universal tool (query and edit) for JSON, YAML, TOML, and XML with a single syntax, similar to `jq`.
  - *Strength:* Converts between formats and edits in place without needing different tools for each file type.
  - *Target Audience:* DevOps engineers dealing with heterogeneous configuration files.

- **sd** (Find & Replace): Intuitive alternative to `sed` for find-and-replace, with much simpler syntax and regex by default.
  - *Strength:* Removes the need to constantly escape special characters, reducing common `sed` mistakes.
  - *Target Audience:* Developers doing quick refactors via terminal.

- **jless** (JSON Viewer): Interactive JSON pager, navigable with VI-style keybindings, optimized for huge JSON files.
  - *Strength:* Collapses/expands deep structures smoothly, outperforming `fx` on very large datasets.
  - *Target Audience:* Backend developers debugging complex API responses.

---

## 🖥️ System and Resource Monitoring

- **bottom (btm)** (Monitoring): Cross-platform system monitor written in Rust, with real-time CPU/memory/network graphs.
  - *Strength:* Extremely customizable via config file, with flexible themes and layouts.
  - *Target Audience:* Developers who want a highly personalizable `htop`/`btop`.

- **nvtop** (GPU Monitoring): The `htop` equivalent for GPUs, displaying usage, temperature, and processes on NVIDIA/AMD/Intel cards.
  - *Strength:* Essential for monitoring AI/ML training workloads in real time, something generic tools don't cover.
  - *Target Audience:* Machine Learning engineers and anyone training models locally.

- **dust (du-dust)** (Disk Usage): Modern alternative to `du`, showing an intuitive visual tree of disk space usage.
  - *Strength:* Instant, readable tree output, without manually combining `du` with `sort`.
  - *Target Audience:* Any terminal user needing to free up space quickly.

- **bandwhich** (Network Monitoring): Shows in real time which process is consuming network bandwidth.
  - *Strength:* Ties network traffic directly to processes and connections, something `iostat`/`htop` don't do.
  - *Target Audience:* System administrators diagnosing abnormal network usage.

- **zenith** (Monitoring): Rust-based system monitor with "zoomable" historical graphs of CPU, memory, network, and disk.
  - *Strength:* Lets you scroll back in time and analyze past usage spikes, not just the current instant.
  - *Target Audience:* SREs investigating performance degradation over time.

---

## ⚡ Productivity, Navigation and Utilities

- **zellij** (Terminal Multiplexer): Modern alternative to `tmux`, with predefined layouts and a gentler learning curve.
  - *Strength:* Discoverable interface with on-screen keybinding hints, reducing the need to memorize commands.
  - *Target Audience:* Developers who find `tmux` unintuitive.

- **yazi** (File Manager): Terminal file manager written in Rust, with async image/video previews.
  - *Strength:* Extremely fast even in directories with thousands of files, with native media previews.
  - *Target Audience:* Power users looking to replace `ranger` with something more performant.

- **atuin** (Shell History): Replaces the default shell history with a searchable SQLite database that syncs across machines.
  - *Strength:* Contextual search (by directory, exit code, time) and encrypted sync between devices.
  - *Target Audience:* Developers working across multiple machines/servers.

- **starship** (Shell Prompt): Customizable, fast, shell-agnostic prompt (Bash, Zsh, Fish, PowerShell).
  - *Strength:* Automatically detects project context (language, Git branch, version) with no complex config.
  - *Target Audience:* Every developer who wants a more informative, better-looking terminal.

- **navi** (Interactive Cheatsheets): Interactive cheatsheet that lets you search for and run complex commands by filling in variables via prompt.
  - *Strength:* Unlike `tldr` (which only displays), `navi` executes the chosen command directly in the terminal.
  - *Target Audience:* Devs who forget flags for complex commands (Docker, ffmpeg, etc.).

---

## 🛠️ Development, Versioning and Automation

- **mise** (Version Manager): Multi-purpose runtime manager (Node, Python, Ruby, Go, etc.), replacing `nvm`, `pyenv`, and `asdf` with a single tool.
  - *Strength:* Much faster than `asdf` (written in Rust) and manages per-project environment variables like `direnv`.
  - *Target Audience:* Full-stack developers switching between multiple languages and projects.

- **difftastic** (Structural Diff): Diff tool that understands code syntax (AST) instead of comparing line by line.
  - *Strength:* Ignores cosmetic changes (formatting, reindentation) and highlights only real semantic changes.
  - *Target Audience:* Developers reviewing pull requests with large refactors.

- **git-delta** (Diff Visualization): Replaces the default `git diff` output with a version featuring syntax highlighting and side-by-side view.
  - *Strength:* Integrates directly with Git/GitHub CLI, making diffs far more readable in the terminal.
  - *Target Audience:* Teams that review code extensively via terminal.

- **tokei** (Code Statistics): Counts lines of code, comments, and blank lines per language, instantly.
  - *Strength:* Extremely fast (Rust) even on massive repositories, supporting 150+ languages.
  - *Target Audience:* Tech leads assessing the size/complexity of a repository.

- **watchexec** (Automation): Automatically runs commands whenever files change, without manually configuring watchers.
  - *Strength:* Language- and stack-agnostic — works for running tests, builds, or linters on any project.
  - *Target Audience:* Developers in live-reload development workflows.

---

## 🤖 AI in the Terminal (New Category)

- **ollama** (Local LLM Execution): CLI for downloading and running open-source language models (Llama, Mistral, Gemma) locally.
  - *Strength:* Abstracts away all the complexity of quantization and inference into a single command (`ollama run`).
  - *Target Audience:* Developers who want local, private, offline AI.

- **llm** (Universal LLM Interface): CLI created by Simon Willison for interacting with multiple models (OpenAI, Anthropic, local) in one place.
  - *Strength:* Supports plugins, embeddings, and conversation logging in SQLite, acting as a unified AI hub.
  - *Target Audience:* Developers testing/comparing multiple LLM providers.

- **aider** (AI Pair Programming): Terminal tool that edits files in a Git repository directly from natural-language instructions.
  - *Strength:* Applies and commits changes automatically, keeping a clean Git history of what the AI changed.
  - *Target Audience:* Developers who want an AI "pair programmer" without leaving the terminal.

- **fabric** (Prompt Automation): Open-source framework that organizes "patterns" (reusable prompts) for tasks like summarizing, extracting insights, or reviewing text via CLI.
  - *Strength:* Creates a reusable, versioned prompt pipeline instead of rewriting prompts from scratch every time.
  - *Target Audience:* Power users automating intellectual workflows with AI.

- **shell-gpt (sgpt)** (Shell Assistant): Integrates language models directly into the shell, generating and explaining commands from natural language.
  - *Strength:* Converts plain-language descriptions directly into ready-to-run shell commands.
  - *Target Audience:* Users who forget complex `find`, `awk`, or `ffmpeg` syntax.
