[English](#english) | [日本語](#日本語)

---

## English

### skills

> A collection of custom skills for [Claude Code](https://claude.ai/code)

Each skill adds focused behaviors to Claude Code — installed by copying a directory into `~/.claude/skills/`.

Browse all skills at **[torifo.github.io/skills](https://torifo.github.io/skills)**

#### Install

```bash
# Clone the individual skill repo and copy the skill directory
git clone https://github.com/torifo/skills-<name> /tmp/skills-<name>
cp -r /tmp/skills-<name>/<name> ~/.claude/skills/
```

#### Skill Catalog

**Git & Version Control**

| Skill | Description |
|-------|-------------|
| [skills-commit](https://github.com/torifo/skills-commit) | Atomic bilingual EN/JA commits with staged file confirmation |
| [skills-changelog](https://github.com/torifo/skills-changelog) | Bilingual changelog generator from git history |
| [skills-safe-commit](https://github.com/torifo/skills-safe-commit) | Pre-commit validator for secrets, AI attribution, and policy violations |
| [skills-branch-cleanup](https://github.com/torifo/skills-branch-cleanup) | Safe stale branch and worktree cleanup with per-deletion confirmation |

**Planning & Execution**

| Skill | Description |
|-------|-------------|
| [skills-plan-before-action](https://github.com/torifo/skills-plan-before-action) | Numbered plan with approval gate before modifying files or running destructive commands |
| [skills-time-estimate](https://github.com/torifo/skills-time-estimate) | Estimates execution time, token usage, and parallelism before heavy operations |
| [skills-run-tests](https://github.com/torifo/skills-run-tests) | Detects test runner, estimates time, offers filter and background options before running |

**Testing & Refactoring**

| Skill | Description |
|-------|-------------|
| [skills-test-gen](https://github.com/torifo/skills-test-gen) | Generates test cases covering happy path, edge cases, and error cases |
| [skills-mock-design](https://github.com/torifo/skills-mock-design) | Adds mocks at correct boundaries — distinguishes when to mock vs use real values |
| [skills-refactor-safe](https://github.com/torifo/skills-refactor-safe) | Refactors with green test baseline — runs tests after each step, reverts on failure |

**Code Quality & Security**

| Skill | Description |
|-------|-------------|
| [skills-dead-code](https://github.com/torifo/skills-dead-code) | Detects unused exports, imports, and functions — confirms each removal |
| [skills-dep-audit](https://github.com/torifo/skills-dep-audit) | Audits dependencies for vulnerabilities, outdated versions, and unused packages |
| [skills-secret-scan](https://github.com/torifo/skills-secret-scan) | Scans files and staged changes for leaked secrets like API keys and tokens |
| [skills-todo-aggregate](https://github.com/torifo/skills-todo-aggregate) | Collects TODO/FIXME/HACK comments into a single report grouped by severity |
| [skills-error-trace](https://github.com/torifo/skills-error-trace) | Systematically analyzes stack traces to extract root cause |

**Database & Performance**

| Skill | Description |
|-------|-------------|
| [skills-sql-explain](https://github.com/torifo/skills-sql-explain) | Analyzes EXPLAIN output and proposes specific query optimizations |
| [skills-mongo-pattern](https://github.com/torifo/skills-mongo-pattern) | Designs MongoDB schemas from access patterns using Computed, Extended Reference, Subset, and Bucket patterns |

**Language Specific**

| Skill | Description |
|-------|-------------|
| [skills-mypy-fix](https://github.com/torifo/skills-mypy-fix) | Fixes mypy/pyright type errors at root cause, preferring narrow types over Any |
| [skills-react-state-review](https://github.com/torifo/skills-react-state-review) | Reviews React state design for derived state, mutation bugs, and missing keys |

---

## 日本語

### skills

> [Claude Code](https://claude.ai/code) 用カスタムスキルのコレクション

各スキルは Claude Code に特定の動作を追加します。`~/.claude/skills/` にディレクトリをコピーしてインストールします。

全スキルの概要は **[torifo.github.io/skills](https://torifo.github.io/skills)** から確認できます。

#### インストール

```bash
# 個別のスキルリポジトリをクローンしてスキルディレクトリをコピー
git clone https://github.com/torifo/skills-<name> /tmp/skills-<name>
cp -r /tmp/skills-<name>/<name> ~/.claude/skills/
```

#### スキル一覧

**Git・バージョン管理**

| スキル | 説明 |
|--------|------|
| [skills-commit](https://github.com/torifo/skills-commit) | ステージ済みファイルを確認しながら英日バイリンガルのアトミックコミットを作成 |
| [skills-changelog](https://github.com/torifo/skills-changelog) | git履歴から英日バイリンガルの更新履歴を生成 |
| [skills-safe-commit](https://github.com/torifo/skills-safe-commit) | コミット前にシークレット・AI帰属・ポリシー違反を検証してブロック |
| [skills-branch-cleanup](https://github.com/torifo/skills-branch-cleanup) | 削除前に確認しながらステールブランチとワークツリーを安全に削除 |

**プランニング・実行**

| スキル | 説明 |
|--------|------|
| [skills-plan-before-action](https://github.com/torifo/skills-plan-before-action) | ファイル変更・破壊的コマンドの前に番号付き計画を提示して承認を待つ |
| [skills-time-estimate](https://github.com/torifo/skills-time-estimate) | 重い操作の前に実行時間・トークン使用量・並列数を見積もる |
| [skills-run-tests](https://github.com/torifo/skills-run-tests) | テストランナーを検出し実行前に時間見積もりとフィルタ・バックグラウンド実行を提案 |

**テスト・リファクタリング**

| スキル | 説明 |
|--------|------|
| [skills-test-gen](https://github.com/torifo/skills-test-gen) | 既存関数の正常系・エッジケース・エラーケースのテストを生成 |
| [skills-mock-design](https://github.com/torifo/skills-mock-design) | 適切な境界にモックを追加。モックすべき箇所と実値を使うべき箇所を判断 |
| [skills-refactor-safe](https://github.com/torifo/skills-refactor-safe) | テスト安全網でリファクタリング。各ステップ後にテスト実行、失敗したら即リバート |

**コード品質・セキュリティ**

| スキル | 説明 |
|--------|------|
| [skills-dead-code](https://github.com/torifo/skills-dead-code) | 未使用のエクスポート・インポート・関数を検出し削除前に確認 |
| [skills-dep-audit](https://github.com/torifo/skills-dep-audit) | 脆弱性・古いバージョン・未使用パッケージを依存関係から検出 |
| [skills-secret-scan](https://github.com/torifo/skills-secret-scan) | APIキーやトークンなどの漏洩したシークレットをスキャン |
| [skills-todo-aggregate](https://github.com/torifo/skills-todo-aggregate) | TODO・FIXME・HACKコメントを深刻度別にまとめたレポートに集約 |
| [skills-error-trace](https://github.com/torifo/skills-error-trace) | スタックトレースを体系的に分析して根本原因を特定 |

**データベース・パフォーマンス**

| スキル | 説明 |
|--------|------|
| [skills-sql-explain](https://github.com/torifo/skills-sql-explain) | EXPLAINの出力を解析し具体的なクエリ最適化を提案 |
| [skills-mongo-pattern](https://github.com/torifo/skills-mongo-pattern) | アクセスパターン駆動でMongoDBスキーマを設計（Computed・Extended Reference・Subset・Bucketパターン） |

**言語固有**

| スキル | 説明 |
|--------|------|
| [skills-mypy-fix](https://github.com/torifo/skills-mypy-fix) | mypy/pyrightの型エラーをroot causeで修正。Anyより狭い型を優先 |
| [skills-react-state-review](https://github.com/torifo/skills-react-state-review) | Reactの状態設計を派生状態・mutationバグ・keyの欠如でレビュー |
