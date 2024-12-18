# Telegram to Markdown Converter

Convert Telegram chat HTML exports to structured Markdown files for LLM analysis.

## Features

- Converts Telegram HTML exports to clean, structured Markdown
- Filters messages by date range
- Splits output into manageable file sizes
- Preserves message metadata and reactions
- Optimized for LLM processing

## Installation

1. Clone the repository:
```bash
git clone https://github.com/YOUR_USERNAME/telegram-markdown-converter.git
cd telegram-markdown-converter
```

2. Install dependencies:
```bash
npm install
```

## Usage

1. Export your Telegram chat history as HTML
2. Place the HTML files in the `messages` directory
3. Run the converter:
```bash
# Basic usage
npm start

# With date range
npm start -- -f 2023-01-01 -t 2023-12-31

# Specify maximum output file size (in KB)
npm start -- -s 1000
```

## Options

- `-f, --from <date>`: Start date (YYYY-MM-DD)
- `-t, --to <date>`: End date (YYYY-MM-DD)
- `-s, --size <size>`: Maximum output file size in KB (default: 500)

## Directory Structure

```
telegram-to-markdown-converter/
├── src/                  # Source code
├── messages/             # Input HTML files
└── output/              # Generated Markdown files
```

## License

MIT

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request
