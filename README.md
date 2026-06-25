# MoonEcho Game Log

GitHub Pages + Jekyll 기반 개인 게임 블로그입니다.

## 로컬 실행

```bash
bundle install
bundle exec jekyll serve
```

브라우저에서 `http://127.0.0.1:4000`으로 확인합니다.

## 새 글 작성

`_posts/`에 `YYYY-MM-DD-title.md` 형식으로 파일을 만들고 front matter를 작성합니다.

```markdown
---
layout: post
title: "글 제목"
date: 2026-06-25 09:00:00 +0900
categories: [리뷰]
tags: [액션, 인디]
excerpt: "목록에 표시될 짧은 설명"
---
```

## 배포

GitHub 저장소를 `moonecho.github.io`로 두고 `main` 브랜치에 푸시하면 GitHub Pages에서 자동 배포됩니다.
