
# Gemini Chatbot with Tools & LangGraph Tracing

This project showcases an agent-based chatbot architecture built with **LangGraph** and enhanced using **Google Gemini API**. It includes modular experiments with tool-augmented agents, Human-in-the-Loop (HITL) interactions, and function calling support. **LangSmith** is integrated for observability and debugging. All implementations are presented as Jupyter Notebooks for transparency and iterative testing.

---

## Features

- Gemini-powered chatbot agents using LangGraph
- Modular agent workflows with stateful execution
- Custom tools (e.g., stock checker, calculator)
- Human-in-the-Loop (HITL) control agents
- LangSmith integration for real-time tracing and debugging
- Clear separation of agents through individual notebooks

---

## Project Structure

```

├── .env                  # Environment variables (empty placeholder)
├── .gitignore
├── README.md
├── requirements.txt      # Auto-generated from your environment
├── uv.lock               # Lockfile (optional, for uv users)
├── agents/               # Agent implementations and routing logic
│   ├── base\_agent.ipynb
│   ├── tools\_agent.ipynb
│   ├── hitl\_agent.ipynb
│   └── ...

````

---

## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/fatimafarhan2/GeminiGraph-Tool-Using-Agents-with-LangGraph.git
cd GeminiGraph-Tool-Using-Agents-with-LangGraph
````

### 2. Create Virtual Environment & Install Dependencies

Using `uv`:

```bash
uv venv
uv pip install -r requirements.txt
```

Or using `pip`:

```bash
python -m venv .venv
source .venv/bin/activate        # On Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Add a `.env` File

Create a `.env` file in the root directory and include:

```env
GOOGLE_API_KEY=
LANGSMITH_TRACING="true"
LANGSMITH_ENDPOINT=
LANGSMITH_API_KEY=
LANGSMITH_PROJECT=
```

These are required for authenticating the Gemini API and enabling LangSmith tracing.

---

## Running the Notebooks

You can open and execute the notebooks using:

```bash
jupyter lab
```

Each notebook demonstrates a unique agent setup powered by LangGraph and Gemini, including support for external tools and HITL configurations.

---

## LangSmith Tracing

LangSmith allows detailed inspection of agent behavior, including node transitions, tool invocations, and error handling. Ensure your `.env` is properly configured for full observability.

---

## Notes

* `.env` is a tracked placeholder; do not commit your actual credentials.
* Artifacts like `.venv` and `.ipynb_checkpoints` are excluded via `.gitignore`.

---

## References

* [LangGraph Documentation](https://docs.langchain.com/langgraph/)
* [LangSmith](https://smith.langchain.com/)
* [Gemini via Google Vertex AI](https://cloud.google.com/vertex-ai)
* [uv Package Manager](https://github.com/astral-sh/uv)

```
