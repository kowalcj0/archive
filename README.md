# My repos archive
-------------------------------------


To recover from selected backup:

```bash
    tar xjf backup.repo.tar.bz2
    git clone backup.repo yourrepo
```

To backup your repo:

```bash
    git clone --mirror yourrepo backup.repo
    tar cjf backup.repo.tar.bz2 backup.repo
    scp backup.tar.bz2 ssh://somewhereelse
```

Based on:
http://superuser.com/a/222765
