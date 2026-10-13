# Changing the past
## 1. Rebasing
```bash
git rebase donut; git rebase baguette; git rebase coffee; git log -1; git switch main
# git log -1으로 확인한 해시의 값을 사용한다. `1e9a03c...`의 위치를 직접 확인한 해시로 변경하면 된다.
git merge --ff-only 1e9a03c
```

## 2. Reordering events
```bash
# 두 가지 방법 중 cherry-pick을 사용한다.
# 나머지 방법은 rebase -i라고 한다.
git checkout main~4; git cherry-pick main~1; git cherry-pick main~2; git cherry-pick main; git cherry-pick main~3
git branch -f main
```
