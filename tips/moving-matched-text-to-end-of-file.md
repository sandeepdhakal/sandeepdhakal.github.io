---
title: Moving matching lines to end of file in vim
date: 2024-03-27
tags: [vim]
---

In vim, we can move all matching lines to the end of the file using the [global command (g)](https://learnvim.irian.to/basics/the_global_command).

Say we have a markdown file with some footenotes througout the file.

```markdown
 ...
 [^angione2022using]: Angione, C., Silverman, E., et al. (2022), Using machine learning as a surrogate model for agent-based simulations.
 
 ...
 
 [^lamperti2018agent]: Lamperti, F., Roventini, A., et al. (2018), Agent-based model calibration using machine learning surrogates.

 ...
```

We can collect these footenotes at the end of the file with:

```vim
:g/^\[\^.*\]:/m $
```

This can be automated every time the file is saved by creating an autocommand. Here's how to create one in NeoVim.

```lua
vim.api.nvim_create_autocmd("BufWritePre", {
    callback = function()
        vim.cmd(":g/^\\[^.*\\]:/m $<CR>")
    end,
    group = vim.api.nvim_create_augroup("markdown_format", { clear = true }),
})

```

Now, everytime the file is saved, any new footnotes added in the file are moved to the bottom.
