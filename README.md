# GoBuster Enhance

[![zread](https://img.shields.io/badge/Ask_Zread-_.svg?style=flat&color=00b0aa&labelColor=000000&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB3aWR0aD0iMTYiIGhlaWdodD0iMTYiIHZpZXdCb3g9IjAgMCAxNiAxNiIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZD0iTTQuOTYxNTYgMS42MDAxSDIuMjQxNTZDMS44ODgxIDEuNjAwMSAxLjYwMTU2IDEuODg2NjQgMS42MDE1NiAyLjI0MDFWNC45NjAxQzEuNjAxNTYgNS4zMTM1NiAxLjg4ODEgNS42MDAxIDIuMjQxNTYgNS42MDAxSDQuOTYxNTZDNS4zMTUwMiA1LjYwMDEgNS42MDE1NiA1LjMxMzU2IDUuNjAxNTYgNC45NjAxVjIuMjQwMUM1LjYwMTU2IDEuODg2NjQgNS4zMTUwMiAxLjYwMDEgNC45NjE1NiAxLjYwMDFaIiBmaWxsPSIjZmZmIi8%2BCjxwYXRoIGQ9Ik00Ljk2MTU2IDEwLjM5OTlIMi4yNDE1NkMxLjg4ODEgMTAuMzk5OSAxLjYwMTU2IDEwLjY4NjQgMS42MDE1NiAxMS4wMzk5VjEzLjc1OTlDMS42MDE1NiAxNC4xMTM0IDEuODg4MSAxNC4zOTk5IDIuMjQxNTYgMTQuMzk5OUg0Ljk2MTU2QzUuMzE1MDIgMTQuMzk5OSA1LjYwMTU2IDE0LjExMzQgNS42MDE1NiAxMy43NTk5VjExLjAzOTlDNS42MDE1NiAxMC42ODY0IDUuMzE1MDIgMTAuMzk5OSA0Ljk2MTU2IDEwLjM5OTlaIiBmaWxsPSIjZmZmIi8%2BCjxwYXRoIGQ9Ik0xMy43NTg0IDEuNjAwMUgxMS4wMzg0QzEwLjY4NSAxLjYwMDEgMTAuMzk4NCAxLjg4NjY0IDEwLjM5ODQgMi4yNDAxVjQuOTYwMUMxMC4zOTg0IDUuMzEzNTYgMTAuNjg1IDUuNjAwMSAxMS4wMzg0IDUuNjAwMUgxMy43NTg0QzE0LjExMTkgNS42MDAxIDE0LjM5ODQgNS4zMTM1NiAxNC4zOTg0IDQuOTYwMVYyLjI0MDFDMTQuMzk4NCAxLjg4NjY0IDE0LjExMTkgMS42MDAxIDEzLjc1ODQgMS42MDAxWiIgZmlsbD0iI2ZmZiIvPgo8cGF0aCBkPSJNNCAxMkwxMiA0TDQgMTJaIiBmaWxsPSIjZmZmIi8%2BCjxwYXRoIGQ9Ik00IDEyTDEyIDQiIHN0cm9rZT0iI2ZmZiIgc3Ryb2tlLXdpZHRoPSIxLjUiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIvPgo8L3N2Zz4K&logoColor=ffffff)](https://zread.ai/YanivHaliwa/gobuster_enhance)
[![deepwiki](https://img.shields.io/badge/Ask_DeepWiki-_.svg?style=flat&color=00b0aa&labelColor=000000&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB3aWR0aD0iMTYiIGhlaWdodD0iMTYiIHZpZXdCb3g9IjAgMCAxNiAxNiIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHJlY3Qgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2IiByeD0iMiIgZmlsbD0iI2ZmZiIvPgo8dGV4dCB4PSI4IiB5PSIxMSIgdGV4dC1hbmNob3I9Im1pZGRsZSIgZm9udC1mYW1pbHk9IkFyaWFsLCBIZWx2ZXRpY2EsIHNhbnMtc2VyaWYiIGZvbnQtc2l6ZT0iNyIgZm9udC13ZWlnaHQ9IjcwMCIgZmlsbD0iIzAwMCI+RFc8L3RleHQ+Cjwvc3ZnPgo%3D&logoColor=ffffff)](https://deepwiki.com/YanivHaliwa/gobuster_enhance)

A Python wrapper that enhances the Gobuster tool with configuration management and improved user experience, making web directory discovery and DNS enumeration faster and more efficient.

## Features

- Easy-to-use CLI interface for Gobuster
- Save and reuse scan configurations with a JSON-based settings system
- Support for both directory (dir) and DNS enumeration modes
- Configurable options for threads, status codes, extensions, and more
- Configuration file editing with your preferred editor (auto-detects $EDITOR environment variable)
- Smart handling of extensions and exclude-length parameters (supports file loading)
- Strong URL validation to prevent errors
- Proper error handling and user feedback
- Secure configuration storage (doesn't store target URLs)

## Prerequisites

- Python 3.x
- Gobuster must be installed and available in your PATH
- Standard wordlists (such as dirbuster's lists, typically found in `/usr/share/wordlists/`)

## Installation

1. Clone the repository using the following command:

```bash 
git clone https://github.com/YanivHaliwa/gobuster_enhance.git
cd gobuster_enhance
```

2. Make the script executable:

```bash
chmod +x gob
```

3. Set up the initial configuration:

```bash
./gob --setup
```

This creates a default configuration file from the template.

## Usage

### Basic Usage

```bash
./gob -u [TARGET_URL] -w [WORDLIST_PATH]
```

Example:

```bash
./gob -u http://example.com -w /usr/share/wordlists/dirbuster/directory-list-2.3-medium.txt
```

When running this command, the tool will prompt you for additional parameters such as mode, threads, status codes, extensions, etc. Your inputs will be saved for future use.

### Using Saved Settings

To use previously saved settings (stored in config.json):

```bash
./gob -j -u [TARGET_URL]
```

This allows you to reuse all your previous configuration parameters with a new target URL.

### Managing Configuration

To edit the configuration file:

```bash
./gob -e
```

This will open the configuration file in your preferred editor (automatically detected from your environment or defaults to common editors).

To reset the configuration to default values:

```bash
./gob --setup
```

## Configuration Options

The tool supports the following configuration options:

- **mode**: Scan mode - either 'dir' for directory scans or 'dns' for DNS enumeration. Default is 'dir'.
- **wordlist**: Path to the wordlist file to use for scanning. Points to dirbuster lists by default.
- **threads**: Number of concurrent threads for scanning. Default is 60 threads.
- **status_code_show**: HTTP status codes to display in results (e.g., "200,301,302,403"). Default shows common response codes (200,301,302,403,401,500).
- **status_code_avoid**: HTTP status codes to hide from results. Used as an alternative to status_code_show.
- **extensions**: File extensions to scan for (comma-separated list like "php,html,js" or path to a file containing extensions). Default includes common web extensions.
- **exclude_length**: Response lengths to exclude from results (comma-separated list or path to a file).
- **cname**: Boolean value (true/false) determining whether to include CNAME records in DNS mode (only applicable for DNS scans).

## Advanced Features

- **Smart Parameter Handling**:

  - For the `extensions` parameter, you can provide a file path instead of typing a long comma-separated list
  - Similarly, for `exclude_length`, you can reference a file containing response lengths to exclude
  - The tool automatically detects if you're providing a file path or direct values
- **Intelligent Editor Detection**:

  - Automatically detects your preferred editor from the `$EDITOR` environment variable
  - Falls back to common editors (nano, vim, emacs, etc.) if $EDITOR is not set
  - Ensures you can always edit your configuration comfortably
- **Secure Configuration Storage**:

  - Target URLs aren't stored in the configuration file for security reasons
  - Only saves parameters that don't contain sensitive information
- **Robust Error Handling**:

  - Validates input parameters to prevent common mistakes
  - Provides clear error messages when something goes wrong
  - Gracefully handles keyboard interrupts and command failures
- **Default Values**:

  - Sensible defaults are used when parameters aren't specified
  - Default extensions include common web file types
  - Default status codes show the most relevant responses

## Security Considerations

- This tool is intended for authorized security testing only
- Always ensure you have permission before scanning any target
- Review the generated commands before execution
- The tool does not store target URLs in the configuration file for security reasons

## License

This project is available under the MIT License.

## Author

Created by [Yaniv Haliwa](https://github.com/YanivHaliwa) for security testing and educational purposes.
