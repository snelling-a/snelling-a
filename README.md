# andrew

## fullstack developer @pipedrive

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

        return Pipedrive
    }

    private openTerminal() {
        return this.terminal
    }

    private openEditor() {
        return this.editor
    }

}
```

```lua
-- me.lua

--- @class SoftwareEngineer
--- @field name string
--- @field editor string
--- @field get_neovim_config fun(self: SoftwareEngineer): string
local M = {}

function M:new(name, editor)
	self = setmetatable({
		name = name,
		editor = editor or "nvim",
	}, {
		__index = self,
	})
	self.name = name
	self.editor = editor

	return self
end

function M:get_neovim_config()
	local config_url = string.format("https://github.com/%s/%s", self.name, self.editor)

	return config_url
end

local andrew = M:new("snelling-a")
local nvim_config = andrew:get_neovim_config()

print(nvim_config) -- https://github.com/snelling-a/nvim

return M
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
