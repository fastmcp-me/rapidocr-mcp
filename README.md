[![Add to Cursor](https://fastmcp.me/badges/cursor_dark.svg)](https://fastmcp.me/MCP/Details/1028/rapidocr)
[![Add to VS Code](https://fastmcp.me/badges/vscode_dark.svg)](https://fastmcp.me/MCP/Details/1028/rapidocr)
[![Add to Claude](https://fastmcp.me/badges/claude_dark.svg)](https://fastmcp.me/MCP/Details/1028/rapidocr)
[![Add to ChatGPT](https://fastmcp.me/badges/chatgpt_dark.svg)](https://fastmcp.me/MCP/Details/1028/rapidocr)
[![Add to Codex](https://fastmcp.me/badges/codex_dark.svg)](https://fastmcp.me/MCP/Details/1028/rapidocr)
[![Add to Gemini](https://fastmcp.me/badges/gemini_dark.svg)](https://fastmcp.me/MCP/Details/1028/rapidocr)

# RapidOCR MCP Server

A MCP server based on RapidOCR, providing an easy-to-use OCR interface.

## Usage

```bash
uvx run rapidocr-mcp
```

## MCP config

```json
"rapidocr-mcp": {
    "command": "uvx",
    "args": [
    "rapidocr-mcp"
    ],
    "env": {}
}
```

## Screenshots

![config](/images/1.png)
![usage](/images/2.png)

## Available Methods

* ocr_by_content
Perform OCR on an image content. Args: base64_data (str): The base64 encoded image content. Returns: List[TextContent]: A list of text content.

* ocr_by_path
Perform OCR on an image file. Args: path (str): The path to the image file. Returns: List[TextContent]: A list of text content.

## remark

Currently, large language models are becoming increasingly powerful and generally possess multimodal capabilities, enabling them to recognize text in images without the need for external OCR tools.