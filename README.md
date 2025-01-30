# 🚀 MojiiCore: Open-Source AI Chat with Frame-Perfect, Live Emojis

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/yourorg/mojiicore/badge)](https://securityscorecards.dev)
[![WebGL 2.0 Rendering](https://img.shields.io/badge/Rendering-60fps_WebGL-green)]()

**Welcome to MojiiCore - Where Conversations Come Alive with Animated Emojis!** 🌍✨

MojiiCore is a **fully open-source** text-based chat platform that brings a new dimension to digital communication. We combine the intelligence of a locally run **DeepSeek-R1 LLM** with **frame-perfect, live emoji animations** powered by **WebAssembly and WebGL** to create engaging, expressive, and human-centered conversations.

<div align="center">
  <img src="docs/demo-preview.gif" width="800" alt="Emojis bursting with life during conversation">
</div>

---

## ✨ Why MojiiCore?

| 🎮 Playful by Design                                       | 🛠️ Professional-Grade Core                                    |
| :-------------------------------------------------------- | :---------------------------------------------------------- |
| 😊 Emojis with personality - laugh, cry, and react like never before | 🔥 WebAssembly-accelerated rendering engine for **frame-perfect** emojis |
| 🎨 Community-created animations and emoji packs             | 🔒 (Optional) Secure communication with robust encryption  |
| 🏆 Earn badges for creative emoji usage                     | 📦 Docker-first production deployment for easy setup        |

---

**MojiiCore** is more than just chat; it's a **dynamic, expressive communication experience** where emojis are not static icons but **living, breathing elements** of your conversations, reacting in real-time to the context and sentiment of your messages!

**Our Vision: Open Source, Expressive Communication for the AI Era**

We believe in the power of open source to create technology that is:

*   **Transparent & Customizable:** Anyone can inspect, modify, and improve MojiiCore's code. We believe in radical transparency, especially as AI becomes more integrated into our lives.
*   **Community-Driven:** Built and shaped by a global community of developers, animators, designers, and emoji enthusiasts. We believe the best ideas come from collaboration.
*   **Privacy-Focused:** Run the AI locally, keeping your data on your own machine.
*   **Engaging & Expressive:** Frame-perfect animated emojis and AI make conversations more human, lively, and fun. We believe digital communication should be as rich and expressive as in-person interactions.
*   **Democratizing Advanced Technology:** We leverage cutting-edge technologies like WebAssembly and WebGL to bring high-performance, delightful experiences to everyone, freely available through open source.

**🔥 Key Features (Open Source & Free):**

*   **Live, Context-Driven Emoji Animations:** Emojis animate in real-time based on the text content and sentiment of the conversation, adding a dynamic visual layer to your chat.
*   **Frame-Perfect 60fps Animations:**  Smooth and responsive animations powered by WebAssembly and WebGL 2.0, ensuring a delightful user experience.
*   **AI-Powered by DeepSeek-R1 (Local):** Engage in intelligent conversations with a locally running, open-source LLM (DeepSeek-R1). Your data stays on your machine.
*   **Modular Architecture:** Easy to extend and customize with your own features and integrations.
*   **Extensible Animation System:**  A framework for creating and adding new emoji animations and trigger rules, driven by the community.
*   **[Add 1-2 more core features, focusing on text-based chat and animations]**

**💎 Premium Features (Future Expansion):**

*   **Advanced Analytics:** Sentiment tracking, detailed conversation reports, and user engagement metrics.
*   **Custom Integrations:** Connect MojiiCore with platforms like Slack, Discord, or other communication tools.
*   **Enterprise Deployment Support:** Options for scalable, secure, and managed deployments for larger organizations.

**🏗️ Architecture Overview:**
mojiicore/
├── config/ # Environment configurations (API keys, etc.)
├── docs/ # Architecture decisions, documentation, demo-preview.gif
├── tests/ # Test suites (unit and integration)
│ ├── integration/
│ └── unit/
├── utils/ # Shared utilities
├── types/ # TypeScript type definitions (if applicable)
├── client/ # Emoji UI + WebAssembly/WebGL + LLM Chat Logic
│ ├── index.html
│ ├── css/
│ │ └── styles.css
│ ├── js/
│ │ ├── emoji-triggers.js # Emoji animation system
│ │ └── deepseek-chat.js # AI chat integration
│ └── wasm/ # Compiled WebAssembly modules for rendering
├── server/ # Python backend (may be optional if using a simple signaling server)
│ ├── deepseek_r1.py # DeepSeek-R1 LLM wrapper (if needed for backend processing)
│ └── [other server files if needed]
├── signaling/ # Signaling server (likely WebSocket-based)
│ └── signaling_server.py
├── models/ # Local model storage
│ └── deepseek-r1-3b/ # Quantized GGUF format of DeepSeek-R1
├── docker-compose.yml # Production deployment configuration
├── LICENSE # Apache 2.0 License
└── requirements.txt # Python dependencies (if any)


**🚀 Getting Started:**

1. **Clone the Repository:**
    ```bash
    git clone [YOUR_REPOSITORY_URL]
    cd mojiicore
    ```

2. **Install Dependencies:**
    ```bash
    # Frontend (adjust commands for your frontend setup)
    cd client
    npm install # or yarn install

    # Backend (if applicable - Python)
    cd ../server
    python3 -m venv .venv
    source .venv/bin/activate # On Windows: .venv\Scripts\activate
    pip install -r requirements.txt
    cd ..
    ```

3. **Download the DeepSeek-R1 Model:**
    ```bash
    # From the mojiicore directory:
    huggingface-cli download TheBloke/deepseek-r1-3B-GGUF --local-dir models/
    ```
    *   **Note:** You'll need to download the specific GGUF quantized version you want to use (e.g., `deepseek-r1-3b.Q4_K_M.gguf`).

4. **Environment Variables:**
    *   Create a `.env` file in the appropriate directory (e.g., `server/` or `client/` depending on where it's needed).
    *   Add your environment variables (if any).
    *   **Important:** `.env` is usually added to `.gitignore` to avoid committing sensitive keys.

5. **Run with Docker Compose (Easiest):**

    ```bash
    docker compose up --build
    # Access at http://localhost:3000
    ```

    Or, run components individually:

    ```bash
    # Start the signaling server (in a separate terminal)
    cd signaling
    python signaling_server.py
    cd ..

    # Start the backend server (if applicable)
    cd server
    python [your_backend_script.py] # e.g., app.py
    cd ..

    # Start the frontend 
    cd client
    npm start # or yarn start, or open index.html directly
    ```

**📜 License:**

MojiiCore is proudly licensed under the **Apache 2.0 License**. We believe in open, accessible technology for everyone. See the `LICENSE` file for details.

**🤝 Contribute to MojiiCore:**

We are actively seeking contributions from developers, designers, animators, AI researchers, and anyone passionate about building a more expressive and engaging communication experience!

*   **Check out our [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.**
*   **Explore the code, especially `emoji-triggers.js`, `deepseek_r1.py` (if applicable), and the `wasm/` modules to understand the core logic.**
*   **Submit issues for bugs or feature requests.**
*   **Join our community discussions!**

**🏆 Community & Credits:**

MojiiCore is currently developed and maintained by [Your Name/Organization Name], but we envision it growing into a vibrant community-driven project. All contributions will be acknowledged and celebrated!

**Join the Conversation:**

*   **Discord:** [YOUR_DISCORD_INVITE_LINK]
*   **GitHub Discussions:** [LINK_TO_YOUR_GITHUB_DISCUSSIONS]

**Let's build the future of humanized, AI-powered communication together!** ✨🚀

