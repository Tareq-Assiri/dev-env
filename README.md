# 🧰 My Dev Setup

This is my personal development environment setup. It includes all the tools I use and my full configuration for each of them.

> ⚠️ **Warning:** This setup will overwrite existing configurations. It's intended for personal use only. Proceed with caution.

## 📁 Repo Structure

```
.
├── .config/        # All my config files (e.g. Neovim, tmux, etc.)
├── .local/         # Local binaries and tools
├── dev             # Script that applies (copies) my config files
├── run             # Main script that runs installation scripts
├── runs/           # Installation scripts for individual tools, executed by `run`
```

## 🚀 Usage

### 1. Clone the Repo

```bash
git clone https://github.com/Tareq-Assiri/dev-setup ~/.dev-setup
cd ~/.dev-setup
```

### 2. Install Tools

Run the installer script to set up all required tools:

```bash
./run
```

This executes all the installation scripts inside `runs/`.

### 3. Preview Config Changes (Safe Step)

Before applying configs, preview what will be overwritten:

```bash
./dev --dry
```

### 4. Apply the Configs (Destructive)

If you are sure, apply the config files:

```bash
./dev
```

This will **overwrite** your existing config files with those in this repo.

## 📝 Notes

- Always install tools first using `run`.
- Use `dev --dry` to safely check config changes before applying.
- Configs are assumed to go under `~/.config` and `~/.local`.
- Designed for use on a fresh Linux machine.
