# cli-tools

A collection of CLI utilities.

## clai

Terminal command assistant powered by Claude via OpenRouter. Converts natural language into exact shell commands.

### Usage

```bash
clai <prompt>
```

Returns the exact shell command you need — no explanation, no markdown.

### Requirements

- Python 3 (pre-installed on macOS)
- An [OpenRouter](https://openrouter.ai) API key

### Setup (new machine)

**1. Clone the repo**

```bash
git clone git@github.com:ChrisEOlsen/cli-tools.git ~/Desktop/repos/cli-tools
```

**2. Make the script executable**

```bash
chmod +x ~/Desktop/repos/cli-tools/clai
```

**3. Add to PATH (pick one)**

Option A — symlink (recommended, picks up future updates automatically):
```bash
ln -s ~/Desktop/repos/cli-tools/clai /usr/local/bin/clai
```

Option B — copy to `/usr/local/bin`:
```bash
cp ~/Desktop/repos/cli-tools/clai /usr/local/bin/clai
```

**4. Set your OpenRouter API key**

Add to `~/.zshrc` (or `~/.bashrc`):
```bash
export OPENROUTER_API_KEY="your_key_here"
```

Then reload your shell:
```bash
source ~/.zshrc
```

**5. Verify**

```bash
clai list all files modified in the last 24 hours
```

### Example output

```
find . -mtime -1 -type f
```
