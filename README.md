# Neon Sign

A cyberpunk-bar color theme for **VS Code**, **Ghostty**, **Starship**, and **zsh**.

Deep violet-black background. Vivid neon syntax — hot pink keywords, electric green functions, violet types, cyan variables. Saturated and punchy, tuned not to burn your retinas.

**[Live preview →](https://twillard22.github.io/neon-sign/)**

---

## Palette

| Token | Hex | Role |
|---|---|---|
| `keyword` | `#ff3d8a` | Keywords, control flow, storage, tags |
| `function` | `#5dff8f` | Functions, methods, aliases |
| `type` | `#b266ff` | Classes, interfaces, enums |
| `variable` | `#5ee2ff` | Variables, properties, JSON keys |
| `string` | `#ffb547` | Strings, parameters (italic) |
| `number` | `#ff7a3d` | Numbers, booleans, null/undefined |
| `special` | `#ff5edb` | Decorators, macros, operators, `this` |
| `bg_main` | `#0f0820` | Editor background |
| `bg_darkest` | `#08040f` | Title bar, terminal, activity bar |
| `fg` | `#e0d4f5` | Default text |
| `fg_dim` | `#6b5a8a` | Comments, placeholders, inactive |

---

## Install

### VS Code

**Via Marketplace (easiest):**

Search `Neon Sign` in the Extensions panel, or:

```
ext install twillard22.neon-sign
```

**Via VSIX:**

1. Download `neon-sign-1.0.0.vsix` from [Releases](https://github.com/twillard22/neon-sign/releases)
2. Run:
   ```bash
   code --install-extension neon-sign-1.0.0.vsix
   ```

### Ghostty

```bash
curl -o ~/.config/ghostty/themes/neon-sign \
  https://raw.githubusercontent.com/twillard22/neon-sign/main/ghostty/neon-sign
```

Then set in your Ghostty config:
```
theme = neon-sign
```

### Starship

```bash
curl -o ~/.config/starship.toml \
  https://raw.githubusercontent.com/twillard22/neon-sign/main/starship/neon-sign.toml
```

### zsh

```bash
# zsh-syntax-highlighting
curl -o ~/.config/zsh/neon-sign-highlights.zsh \
  https://raw.githubusercontent.com/twillard22/neon-sign/main/zsh/zsh-highlights.zsh

# zsh-autosuggestions
curl -o ~/.config/zsh/neon-sign-autosuggest.zsh \
  https://raw.githubusercontent.com/twillard22/neon-sign/main/zsh/zsh-autosuggest.zsh
```

Then source both files in your `.zshrc` **before** the plugin sources:

```zsh
source ~/.config/zsh/neon-sign-autosuggest.zsh
source ~/.config/zsh/neon-sign-highlights.zsh

source $(brew --prefix)/share/zsh-autosuggestions/zsh-autosuggestions.zsh
source $(brew --prefix)/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
```

---

## License

MIT
