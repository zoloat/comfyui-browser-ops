# comfyui-browser-ops

Claude in Chrome(ブラウザ拡張機能)と Claude Code を組み合わせて、ComfyUI を運用した記録です。

- 上層: Chrome 拡張機能上の Claude が、ComfyUI の画面を操作して試行錯誤する
- 下層: Claude Code が、環境構築・ファイル・シェルを担当する
- 人間: 2つの層を直接つながず、依頼を確認して中継する

詳しい考え方はブログに書きます(公開後にリンクを追加します)。

## 中身

| ファイル | 内容 |
|---|---|
| [SKILL.md](SKILL.md) | 役割分担と、人間の承認が必要な場面 |
| [docs/roles.md](docs/roles.md) | 上層・下層・人間の責務 |
| [docs/approval.md](docs/approval.md) | カスタムノード導入時に確認する項目 |
| [docs/risks.md](docs/risks.md) | 想定リスクと対策 |
| [docs/prior-art.md](docs/prior-art.md) | 先行例の調査(2026-10-20 時点) |
| [templates/handoff.md](templates/handoff.md) | 上層から下層への依頼書の書式 |

## 注意

- 確認した日付: 2026-10-20。拡張機能・ComfyUI ともに仕様が変わりやすいので、日付を確認してから使ってください。
- 自分の環境で使う前に [docs/risks.md](docs/risks.md) を読んでください。
