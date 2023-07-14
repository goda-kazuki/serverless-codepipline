# serverless-codepipline


## 複数のリポジトリにプッシュしたい場合

```text:.git/config
[core]
        repositoryformatversion = 0
        filemode = true
        bare = false
        logallrefupdates = true
[remote "origin"]
        url = https://github.com/goda-kazuki/serverless-codepipline.git
        fetch = +refs/heads/*:refs/remotes/origin/*
        url = https://git-codecommit.ap-northeast-1.amazonaws.com/v1/repos/{リポジトリ名}
[branch "main"]
        remote = origin
        merge = refs/heads/main
```