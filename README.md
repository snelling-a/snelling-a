# andrew

## fullstack developer

```typescript
// me.ts

class Andrew extends SoftwareEngineer {
    constructor (
        private readonly terminal: WezTerm,
        public editor: Neovim
    )

    public job() {
        wakeUp()

        this.openTerminal()

        this.openEditor()

        work()
    }

    private openTerminal() {
        return this.terminal
    }

    private openEditor() {
        return this.editor
    }

}
```

```bash
#!/usr/bin/env bash
# env.sh
# downloads dotfiles and sets up the dev environment

DOTFILES="$HOME/dotfiles"
git clone git@github.com:snelling-a/dotfiles.git "$DOTFILES"

"$DOTFIELS/install.sh"

echo "Installing node..."
echo "Installing typescript..."
echo "Installing deno..."
echo "Installing lua..."

echo "Happy hacking!"
```

[**octo ring**](https://octo-ring.com/)  
[[prev](https://octo-ring.com/p/hedyhli/prev)]  [[random](https://octo-ring.com/p/hedyhli/random)]  [[next](https://octo-ring.com/p/hedyhli/next)]
