# jitsubutsu-comment

Claude Code 用のスキルです。Claude が作った見た目のある成果物（LP・画面・メールや LINE の文面・資料・スライドなど）を、**実際に使われる場所に近い見た目**の claude.ai Artifact にして、スマホから開ける URL で渡します。

- **コメント**：ページ右下の「コメント」から、気になる箇所をタップして指示を書き、Send to Claude を押すと、Claude が直して同じ URL に出し直します
- **意図**：ページ右下の「意図」を押すと、Claude が各所をなぜそう作ったかが出ます（普段は非表示）

## 必要なもの

- Claude Code（Artifact を publish できる環境。claude.ai にログインしていること）
- Artifact のコメント機能（`comments` capability）が使えるアカウント

## 入れ方

```bash
git clone https://github.com/maokao96/jitsubutsu-comment ~/.claude/skills/jitsubutsu-comment
```

プロジェクトだけで使う場合は `<プロジェクト>/.claude/skills/jitsubutsu-comment` に置いてください。

## 使い方

Claude Code で次のように頼みます。

- 「この LP を実物で見せて」
- 「メール文面、スマホで確認したい」
- `/jitsubutsu-comment`

見た目のある成果物を作ったときは、頼まなくてもこの形で渡すようになります。

## 中身

- `SKILL.md` — スキル本体（Claude への手順）
- `template.html` — 舞台（メール・チャット・スマホ・紙・スライドの枠）と、コメント・意図の二つのボタンを入れた雛形

## ライセンス

MIT
