
```
# Gemini Chatbot with Tools & LangSmith Tracing

This project demonstrates how to build an agent-based chatbot using **LangChain**, **Google Gemini API**, and **LangSmith** for observability. It includes experiments with tool-augmented agents, Human-in-the-Loop (HITL) control, and Gemini function calling. All implementations are provided as Jupyter Notebooks for transparency and experimentation.

---

## Features

- Gemini-powered chatbot built with LangChain
- Custom tools (e.g., stock price retriever, calculator)
- Human-in-the-Loop (HITL) agent control
- LangSmith integration for tracing and debugging
- Interactive `.ipynb` notebooks for modular testing

---

## Project Structure

```

├── .env # Environment variables (empty placeholder)
├── .gitignore
├── README.md
├── requirements.txt # Auto-generated from your environment
├── uv.lock # Lockfile (optional, for uv users)
├── agents/ # Agent implementations and routing logic
│ ├── base_agent.ipynb
│ ├── tools_agent.ipynb
│ ├── hitl_agent.ipynb
│ └── ...

````

---

## Setup Instructions

### 1. Clone the Repository

```bash
git clone [https://github.com/your-username/gemini-chatbot-langchain.git](https://github.com/fatimafarhan2/GeminiGraph-Tool-Using-Agents-with-LangGraph)
cd gemini-chatbot-langchain
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
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Add a `.env` File

Create a `.env` file in the root directory and add the following environment variables:

```env
GOOGLE_API_KEY=
LANGSMITH_TRACING="true"
LANGSMITH_ENDPOINT=
LANGSMITH_API_KEY=
LANGSMITH_PROJECT=
```

---

## Running the Notebooks

You can open and execute the notebooks using Jupyter:

```bash
jupyter lab
```

Each notebook focuses on a different type of agent setup or LangChain feature.

---

## LangSmith Tracing

LangSmith is integrated to help visualize the agent's tool usage, decision-making, and chain execution. Make sure your `.env` is correctly configured for full observability.

---

## Notes

* `.env` is intentionally tracked as a placeholder (do not commit actual secrets).
* `.venv`, `.ipynb_checkpoints`, and other build artifacts are excluded via `.gitignore`.

---

## References

* [LangChain Documentation](https://docs.langchain.com/)
* [LangSmith](https://smith.langchain.com/)
* [Gemini via Google Vertex AI](https://cloud.google.com/vertex-ai)
* [uv Package Manager](https://github.com/astral-sh/uv)

```


