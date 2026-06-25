# AGENTS.md

이 저장소는 GitHub Pages로 배포되는 Jekyll 기반 개인 게임 블로그입니다.

## 프로젝트 구조

- `_config.yml`: 사이트 제목, 설명, URL, 플러그인, permalink 설정
- `_layouts/default.html`: 전체 페이지 공통 레이아웃
- `_layouts/post.html`: 블로그 글 레이아웃
- `assets/css/style.css`: 사이트 디자인
- `assets/images/`: 블로그에서 사용하는 이미지 자산
- `index.md`: 홈 화면
- `about.md`: 소개 페이지
- `_posts/`: 블로그 글
- `Gemfile`: GitHub Pages/Jekyll 의존성

## 글 작성 규칙

새 글은 `_posts/` 아래에 만듭니다.

파일명 형식:

```text
YYYY-MM-DD-post-title.md
```

예시:

```text
2026-06-25-night-play-log.md
```

글 상단에는 YAML front matter를 넣습니다.

```markdown
---
layout: post
title: "글 제목"
date: 2026-06-25 09:00:00 +0900
categories: [플레이로그]
tags: [일지, 탐험]
excerpt: "목록에 표시될 짧은 설명"
---
```

## 로컬 미리보기

Ruby와 Bundler가 설치된 환경에서 실행합니다.

```bash
bundle install
bundle exec jekyll serve
```

브라우저에서 `http://127.0.0.1:4000`을 열어 확인합니다.

## 배포

- GitHub 저장소 이름은 보통 `moonecho.github.io`를 사용합니다.
- GitHub Pages 설정은 `Settings -> Pages`에서 확인합니다.
- `main` 브랜치에 푸시하면 GitHub Pages가 자동으로 빌드하고 배포합니다.

## 작업 원칙

- 커스텀 레이아웃과 `assets/css/style.css` 중심으로 디자인을 유지합니다.
- 글 파일은 한국어 본문과 명확한 제목을 우선합니다.
- `_config.yml`을 수정할 때는 `url`, `baseurl`, 플러그인, permalink가 GitHub Pages와 호환되는지 확인합니다.
- 새로 만든 파일은 작업 후 `git add`까지 진행합니다.
- 불필요한 빌드 결과물, 캐시, 임시 파일은 커밋하지 않습니다.
