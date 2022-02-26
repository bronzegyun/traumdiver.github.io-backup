---
layout: default
title: Useful Git commands
---
# 알아두면 좋은 깃 명령어 모음
{: .no_toc }
평소 `GitKraken`이란 앱을 사용하지만, 가끔 먹통이 되거나 느릴때 깃 명령어를 사용함.  
**깃 명령어 사용시 장점**은 앱에서 지원하지 않는 기능을 사용할 수 있고, 관련 로그를 콘솔을 통해 볼 수 있음.  
가끔 기억이 안 나는 경우를 대비해 깃 명령어를 정리함.

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## 브랜치 관련

### 브랜치 삭제
대상 브랜치를 삭제함.
```
$ git branch -d master
```

### 브랜치 이름 변경
현재 체크아웃돼 있는 브랜치의 이름을 변경함.
```
$ git branch -m master
```

### 독립된 브랜치(orphan branch) 생성
기존 히스토리를 공유하지 않는 새로운 브랜치를 생성함.
```
$ git checkout --orphan latest_branch
```