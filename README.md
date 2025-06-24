## 🚀 Zsh Setup: Oh My Zsh, Plugins, and Starship with Nerd Font Symbols

### 📌 Steps

```bash
# 1️⃣ Install Oh My Zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

# 2️⃣ Install recommended Zsh plugins

# zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-autosuggestions $ZSH_CUSTOM/plugins/zsh-autosuggestions

# zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting

# fzf (Fuzzy Finder)
git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf
~/.fzf/install

# zsh-completions
git clone https://github.com/zsh-users/zsh-completions $ZSH_CUSTOM/plugins/zsh-completions

# 3️⃣ Install Starship prompt and Nerd Font Symbols preset

# Install Starship
curl -sS https://starship.rs/install.sh | sh

# Generate Nerd Font Symbols preset
starship preset nerd-font-symbols -o ~/.config/starship.toml

# 4️⃣ Add Starship init to the end of your ~/.zshrc
# (Add this line at the bottom)
# eval "$(starship init zsh)"

# 5️⃣ Use a Nerd Font in your terminal to see all icons properly!
# (e.g., FiraCode Nerd Font, JetBrains Mono Nerd Font, etc.)
