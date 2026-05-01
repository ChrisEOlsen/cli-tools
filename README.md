# cli-tools

A collection of CLI utilities.

## clai

Terminal command assistant powered by Claude via OpenRouter.

### Usage

```bash
clai <prompt>
```

Returns the exact shell command you need — no explanation, no markdown.

### Setup

1. Install: copy `clai` to somewhere on your `$PATH` (e.g. `/usr/local/bin/clai`) and `chmod +x` it
2. Set env var: `export OPENROUTER_API_KEY=your_key_here`

### Example

```bash
clai list all files modified in the last 24 hours
```
