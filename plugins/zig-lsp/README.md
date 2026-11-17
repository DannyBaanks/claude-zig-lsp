# zig-lsp

Claude Code plugin that connects the Zig language server [zls](https://github.com/zigtools/zls) for `.zig` and `.zon` files.

## Requirements

`zls` on `PATH`, built for the same Zig version you use (zls 0.16.x for Zig 0.16, 0.17.x for Zig 0.17).
Fork with the pinned branch: https://github.com/DannyBaanks/zls (`isy/0.16`).

```bash
git clone -b isy/0.16 https://github.com/DannyBaanks/zls && cd zls
zig build -Doptimize=ReleaseSafe && install -m755 zig-out/bin/zls ~/.local/bin/zls
```

## Install

```bash
claude plugin marketplace add DannyBaanks/claude-zig-lsp
claude plugin install zig-lsp@isy-plugins
```
