# ギット・フック

- [バージョン管理](../../readme.md)
- [バージョン管理／ギット／フック](readme.md)

## コミット・メッセージ（commit_message）

### 実装方法

バッシュを利用する場合、以下の命令文をギット・リポジトリ内で実行してください。

``` bash
if git rev-parse --is-inside-work-tree | grep --regexp="^true" --quiet; then curl --output "$(git rev-parse --show-toplevel)/.git/hooks/commit-msg" https://raw.githubusercontent.com/possior/VERSION_CONTROL/Default/Git/Hooks/commit_message && chmod +x "$(git rev-parse --show-toplevel)/.git/hooks/commit-msg"; fi
```

# Git Hooks

- [Version Control](../../readme.md)
- [Version Control / Git / Hooks](readme.md)

## Commit Message (commit_message)

### Deployment

If you would like to use Bash, execute the following command inside the git repository.

``` bash
if git rev-parse --is-inside-work-tree | grep --regexp="^true" --quiet; then curl --output "$(git rev-parse --show-toplevel)/.git/hooks/commit-msg" https://raw.githubusercontent.com/possior/VERSION_CONTROL/Default/Git/Hooks/commit_message && chmod +x "$(git rev-parse --show-toplevel)/.git/hooks/commit-msg"; fi
```
