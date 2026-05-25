# Neon Sign

A cyberpunk-bar color theme for **VS Code**, **Ghostty**, **Starship**, and **zsh**.

Two variants:

- **Neon Sign** — deep violet-black background, full-saturation neons. Hot pink keywords, electric green functions, violet types, cyan variables. Loud and punchy.
- **Neon Sign Muted** — same hue identity at ~30% lower saturation, lifted plum background. Calmer for long sessions.

**[Live preview →](https://twillard22.github.io/neon-sign/)**

---

## Palettes

### Neon Sign (vivid)

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

### Neon Sign Muted (calmer)

| Token | Hex | Role |
|---|---|---|
| `keyword` | `#e87aa8` | Softer pink |
| `function` | `#8de0a5` | Sage green |
| `type` | `#b896d8` | Soft violet |
| `variable` | `#8fcde0` | Soft cyan |
| `string` | `#e8c074` | Warm amber |
| `number` | `#e89870` | Soft orange |
| `special` | `#d090c8` | Soft magenta |
| `bg_main` | `#1e1830` | Editor background |
| `bg_darkest` | `#161025` | Title bar, terminal, activity bar |
| `fg` | `#d8cee8` | Default text |
| `fg_dim` | `#8a7ba8` | Comments, placeholders, inactive |

---

## Install

### VS Code

**Via Marketplace (easiest):**

Search `Neon Sign` in the Extensions panel, or:

```
ext install twillard22.neon-sign
```

Both variants (Neon Sign and Neon Sign Muted) are included in the same extension. Select your preferred variant via **File → Preferences → Color Theme**.

**Via VSIX:**

1. Download `neon-sign-1.1.0.vsix` from [Releases](https://github.com/twillard22/neon-sign/releases)
2. Run:
   ```bash
   code --install-extension neon-sign-1.1.0.vsix
   ```

### Ghostty

```bash
# Vivid
curl -o ~/.config/ghostty/themes/neon-sign \
  https://raw.githubusercontent.com/twillard22/neon-sign/main/ghostty/neon-sign

# Muted
curl -o ~/.config/ghostty/themes/neon-sign-muted \
  https://raw.githubusercontent.com/twillard22/neon-sign/main/ghostty/neon-sign-muted
```

Then set in your Ghostty config:
```
theme = neon-sign
# or:
theme = neon-sign-muted
```

### Starship

```bash
# Vivid
curl -o ~/.config/starship.toml \
  https://raw.githubusercontent.com/twillard22/neon-sign/main/starship/neon-sign.toml

# Muted
curl -o ~/.config/starship.toml \
  https://raw.githubusercontent.com/twillard22/neon-sign/main/starship/neon-sign-muted.toml
```

### zsh

```bash
# Vivid — zsh-syntax-highlighting
curl -o ~/.config/zsh/neon-sign-highlights.zsh \
  https://raw.githubusercontent.com/twillard22/neon-sign/main/zsh/zsh-highlights.zsh

# Vivid — zsh-autosuggestions
curl -o ~/.config/zsh/neon-sign-autosuggest.zsh \
  https://raw.githubusercontent.com/twillard22/neon-sign/main/zsh/zsh-autosuggest.zsh

# Muted — zsh-syntax-highlighting
curl -o ~/.config/zsh/neon-sign-muted-highlights.zsh \
  https://raw.githubusercontent.com/twillard22/neon-sign/main/zsh/neon-sign-muted-highlights.zsh

# Muted — zsh-autosuggestions
curl -o ~/.config/zsh/neon-sign-muted-autosuggest.zsh \
  https://raw.githubusercontent.com/twillard22/neon-sign/main/zsh/neon-sign-muted-autosuggest.zsh
```

Then source both files in your `.zshrc` **before** the plugin sources:

```zsh
source ~/.config/zsh/neon-sign-autosuggest.zsh      # or -muted-
source ~/.config/zsh/neon-sign-highlights.zsh        # or -muted-

source $(brew --prefix)/share/zsh-autosuggestions/zsh-autosuggestions.zsh
source $(brew --prefix)/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
```

---

## License

MIT
