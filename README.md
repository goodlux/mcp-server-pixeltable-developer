# Pixeltable stio MCP Server

**Claude meets Pixeltable.** The AI multimodal database, now available as an MCP server.

## ⚡ Quick Start

```bash
git clone https://github.com/yourusername/mcp-server-pixeltable
cd mcp-server-pixeltable
uv sync
```

Add to your Claude Desktop config:

```json
{
  "mcpServers": {
    "pixeltable": {
      "command": "uv",
      "args": [
        "run",
        "--directory",
        "{path-to-your-repo}",
        "python",
        "-m",
        "mcp_server_pixeltable"
      ],
      "env": {
        "PIXELTABLE_HOME": "/Users/{your-username}/.pixeltable",
        "PIXELTABLE_FILE_CACHE_SIZE_G": "10"
      }
    }
  }
}
```

## 🚀 What You Get

- **Multimodal AI Database** - Images, audio, video, documents in one place
- **Local LLM Integration** - Ollama, Llama.cpp, Whisper, YOLOX 
- **Zero API Costs** - Everything runs locally
- **UV-Powered Dependencies** - Automatic package management
- **Production Ready** - Built on Pixeltable's robust foundation

## 💡 Examples

**Create and populate a table:**
```
Claude: Create a table for my screenshots
Claude: Add object detection to all images
Claude: Transcribe any audio files with Whisper
```

**Local AI analysis:**
```
Claude: Use Ollama to analyze these images
Claude: Generate embeddings for semantic search
Claude: Run YOLOX object detection on my photos
```

**Data workflows:**
```
Claude: Show me all images with cars detected
Claude: Find documents mentioning "AI"
Claude: Create a summary of this video
```

Built while having coffee. ☕

---

*Requires Claude Desktop and Pixeltable. Works with any local LLM via Ollama.*