# confirm_default_branch_changed_main
そういえば github のデフォルトブランチが main に変わったはずなのでチェックしてみる

```
# 元々は
alias gr='git fetch --prune --all && git checkout origin/master && git plog -10 && git status'

# BLM に端を発して default branch を master から main に変更する流れがあり
alias gr='git fetch --prune --all && git checkout origin/main && git plog -10 && git status'

# とすると、リポジトリ毎に設定するのが面倒だし、ということで
alias gr='git fetch --prune --all && git checkout origin/HEAD && git plog -10 && git status'

で、どうにかならないかなと。

```
