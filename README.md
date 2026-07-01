# AI駆動開発時代のNeovim（Zenn Book）

Mac（Apple Silicon）で Neovim 0.12 + tmux + Ghostty の開発環境を組み、**自前のローカル LLM（Ollama）に SSH 越しで繋いでエージェントと協働する**ところまでを扱う Zenn Book のソース。

汎用 Neovim 入門ではなく、**ローカル LLM と組む「AI 駆動開発の土俵」づくり**に特化する（基礎の深掘りは既存良書へ譲る）。

## 構成（Zenn Book）

```
books/neovim-ide-on-mac/
├── config.yaml          # タイトル/トピック/章順（published:false・¥0）
├── intro / overview     # はじめに・全体像（AI駆動IDEの位置づけ・0.12前提）
├── terminal-ghostty / tmux / neovim-ide / neovim-tmux   # 土台（圧縮）
├── remote-dev / neovim-llm / agent-pair                 # ★主役：ローカルLLM接続
├── outro                # おわりに・姉妹本導線
└── cheatsheet           # 付録：早見表
```

## プレビュー（zenn-cli）

```sh
npm install zenn-cli@latest
npx zenn preview
```

## 補足

- 旧 `docs/`（VitePress 検討時の名残）は不要。`git rm -r docs` で除去のこと。
- 本書は L1（Tips）。Neovim 0.12 世代のスナップショットとして扱う。
