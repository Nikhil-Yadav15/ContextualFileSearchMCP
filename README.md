# 📂 Contextual File Searcher MCP🚀

This Python-based tool helps you find the most relevant files on your computer using smart content search. Instead of just checking for filenames, it digs into the actual content of the files and ranks them based on how closely they match your search query. 💡

---

## ✨ Key Features

* 🔍 **Smart Search**: Combines keyword match and semantic similarity using `sentence-transformers`.
* 📄 **Multiple File Types**: Supports `.pdf`, `.docx`, `.txt`, `.py`, `.csv`, `.xlsx`, `.xls` and more.
* ⚡ **Fast & Efficient**: Limits long files and chunks text for better performance.
* 🧠 **Intelligent Scoring**: Uses a hybrid scoring formula to balance keywords and meaning.

---

## 🛠️ How It Works

1. **Input**: Provide a folder path and your search query.
2. **Processing**:

   * Extracts text from all supported files.
   * Chunks the text and calculates keyword frequency.
   * Computes semantic similarity using a pre-trained transformer model.
3. **Ranking**: Files are scored and ranked by relevance.
4. **Output**: Shows top results with similarity score and keyword count.

---

## ▶️ Getting Started

### 1. Clone the Repo

```bash
git clone https://github.com/Nikhil-Yadav15/ContextualFileSearchMCP.git
```

### 2. Add Dependencies Using uv

```bash
uv init
uv add sentence-transformers PyPDF2 python-docx openpyxl mcp[cli]
```

### 3. Run the MCP Tool

```bash
uv run mcp install SearchFileByContent.py
```

---

# 🧪 Usage

Once the server is running, you can interact with it using the defined tools. For example:

## Search for Files

Invoke the `search_files_by_content` tool with parameters like:
- Drive letter
- File extension
- Content hint

The server will return JSON-formatted results, including:
- File paths
- Relevance scores
- Content previews

## List Available Drives

Use the `list_drives` tool to view all accessible disk drives on your system.


---

## 📚 Requirements

* Python 3.8+
* `sentence-transformers`
* `PyPDF2`, `python-docx`, `openpyxl`, `pandas`

---

