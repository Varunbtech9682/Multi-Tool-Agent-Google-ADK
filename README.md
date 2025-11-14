# Multi-Tool-Agent-Google-ADK

<h1>🚀 Multi Tool Agent – Google ADK Sample Project</h1>

<p>A simple multi-tool AI agent built using Google's Agent Development Kit (ADK). This project demonstrates how to create an agent that can answer queries about weather and current time using custom Python tools.
</p>

<p>
  <img src="https://img.shields.io/github/repo-size/Varunbtech9682/Multi-Tool-Agent-Google-ADK" />
  <img src="https://img.shields.io/github/contributors/Varunbtech9682/Multi-Tool-Agent-Google-ADK" />
  <img src="https://img.shields.io/github/license/Varunbtech9682/Multi-Tool-Agent-Google-ADK" />
  <img src="https://img.shields.io/badge/Python-3.9+-blue" />
  <img src="https://img.shields.io/badge/Google-ADK-orange" />
  <img src="https://img.shields.io/badge/PRs-welcome-brightgreen" />
</p>

<p>
A simple multi-tool AI Agent built using <strong>Google’s Agent Development Kit (ADK)</strong>.
This project demonstrates how to build custom tools (functions) and integrate them into an AI agent.
</p>

<ul>
  <li>🌤 Weather lookup</li>
  <li>⏰ Current time lookup</li>
  <li>🔌 API key-based authentication</li>
  <li>🧪 ADK Dev UI debugging</li>
  <li>🧠 Flexible agent architecture</li>
</ul>

<hr />

<h2>📸 Screenshots</h2>



<h3>🔹 ADK Dev UI</h3>
<img src="https://image2url.com/images/1763053516976-7be9c0a5-6a5c-4f4a-8264-5dc42ca806a1.png" alt="Dev UI Screenshot" />

<h3>🔹 Tool Execution Log</h3>
<div style="margin:0; height:300px ; width: 300px; display:flex; justify-content:center; align-items:center;">
  <img src="https://image2url.com/images/1763053580564-d5b583f6-321c-46d7-a6ec-16176f2f7b48.png"
       alt="Tool Log"
       style="max-width:100%; height:500px;" />

</div>

<hr />

<h2>📁 Project Structure</h2>

<pre>
Multi_tool_agent/
│
├── multi_tool_agent/
│   ├── __init__.py
│   ├── agent.py
│   ├── .env
│
└── README.md
</pre>

<hr />

<h2>🛠 Installation</h2>

<h3>1️⃣ Clone the repository</h3>

<pre><code>git clone https://github.com/your-username/Multi_tool_agent.git
cd Multi_tool_agent
</code></pre>

<h3>2️⃣ Create & activate a virtual environment (Windows)</h3>

<pre><code>python -m venv .venv
.venv\Scripts\activate
</code></pre>

<h3>3️⃣ Install dependencies</h3>

<pre><code>pip install google-adk
</code></pre>

<hr />

<h2>🔧 Configuration</h2>

<p>Create a <code>.env</code> file inside:</p>

<pre>multi_tool_agent/.env</pre>

<p>Add:</p>

<pre><code>GOOGLE_GENAI_USE_VERTEXAI=FALSE
GOOGLE_API_KEY=YOUR_API_KEY_HERE
</code></pre>

<p>API Key from: <a href="https://aistudio.google.com/">https://aistudio.google.com/</a></p>

<hr />

<h2>▶️ Running the Agent</h2>

<p>Start the development UI:</p>

<pre><code>adk web --no-reload
</code></pre>

<p>Then open:</p>

<pre>http://localhost:8000</pre>

<p>Select <strong>multi_tool_agent</strong> from the dropdown.</p>

<hr />

<h2>🧪 Example Prompts</h2>

<ul>
  <li>What is the weather in New York?</li>
  <li>What is the time in New York?</li>
  <li>What is the weather in Paris?</li>
  <li>What is the time in Tokyo?</li>
</ul>

<hr />

<h2>🧱 Architecture Diagram</h2>

🧱 Architecture Diagram
<pre>
              ┌───────────────────────┐
              │      User Query       │
              └───────────┬───────────┘
                          │
                ┌─────────▼───────────┐
                │       ADK Agent     │
                │ model: gemini-flash │
                └─────────┬───────────┘
                          │
          ┌───────────────▼────────────────┐
          │     Tool Execution Layer       │
          │  • get_weather(city)           │
          │  • get_current_time(city)      │
          └───────────────┬────────────────┘
                          │
                ┌─────────▼─────────┐
                │   Tool Response   │
                └─────────┬─────────┘
                          │
                ┌─────────▼─────────┐
                │   Final Answer    │
                └───────────────────┘

  </pre>

<hr />

<h2>🤝 Contributing</h2>

<p>
Contributions, issues, and feature requests are welcome!  
Feel free to open a Pull Request.
</p>

<hr />

<h2>📄 License</h2>

<p>This project is licensed under the <strong>MIT License</strong>.</p>

<hr />

<h2>⭐ Support</h2>

<p>If this project helped you, please give it a <strong>star ⭐ on GitHub</strong>!</p>
