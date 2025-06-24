# 🚀 Zsh Setup — Oh My Zsh, Plugins, and Starship with Nerd Font Symbols

A quick guide to set up a modern Zsh environment with useful plugins and a beautiful Starship prompt.

---

## 1️⃣ Install Oh My Zsh

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

---

## 2️⃣ Install Recommended Zsh Plugins

### zsh-autosuggestions

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions
```

### zsh-syntax-highlighting

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
```

### fzf (Fuzzy Finder)

```bash
git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf
~/.fzf/install
```

### zsh-completions

```bash
git clone https://github.com/zsh-users/zsh-completions $ZSH_CUSTOM/plugins/zsh-completions
```

---

## 3️⃣ Install Starship Prompt and Nerd Font Symbols Preset

### Install Starship

```bash
curl -sS https://starship.rs/install.sh | sh
```

### Apply Nerd Font Symbols Preset

```bash
starship preset nerd-font-symbols -o ~/.config/starship.toml
```

---

## 4️⃣ Add Starship to your `.zshrc`

Add this line at the **end** of your `~/.zshrc` file:

```bash
eval "$(starship init zsh)"
```

---

## ✅ Done!

- Restart your terminal or run `source ~/.zshrc`
- Make sure your terminal font is a Nerd Font (e.g., FiraCode Nerd Font, JetBrains Mono Nerd Font) to see all icons properly.
