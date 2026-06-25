# AGENTS.md

이 저장소는 GitHub Pages로 배포되는 Jekyll 기반 개인 사이트입니다. 게임 스트리머 달빛여운의 와우 자료실과 클래스별 가이드를 중심으로 운영합니다.

## 프로젝트 구조

- `_config.yml`: 사이트 제목, 설명, URL, 플러그인, permalink 설정
- `_layouts/default.html`: 전체 페이지 공통 레이아웃
- `_layouts/post.html`: 필요 시 사용하는 글 레이아웃
- `assets/css/style.css`: 사이트 디자인
- `assets/images/`: 사이트에서 사용하는 이미지 자산
- `assets/downloads/`: 폰트, 설정 파일 같은 다운로드 자산
- `index.md`: 홈 화면
- `wow.md`: 월드 오브 워크래프트 자료실
- `classes.md`: 클래스별 가이드 허브
- `about.md`: 소개 페이지
- `_posts/`: 필요 시 남기는 기록 글
- `Gemfile`: GitHub Pages/Jekyll 의존성

## 콘텐츠 작성 규칙

사이트형 콘텐츠는 일반 페이지로 만듭니다.

예시:

```markdown
---
layout: default
title: 페이지 제목
permalink: /example/
---
```

블로그식 기록 글이 필요할 때만 `_posts/` 아래에 만듭니다.

파일명 형식:

```text
YYYY-MM-DD-post-title.md
```

## 로컬 미리보기

Ruby와 Bundler가 설치된 환경에서 실행합니다.

```bash
bundle install
bundle exec jekyll serve
```

브라우저에서 `http://127.0.0.1:4000/moonecho/`를 열어 확인합니다.

## 배포

- 현재 배포 주소는 `https://flat81.github.io/moonecho/`입니다.
- `_config.yml`의 `baseurl: "/moonecho"`는 GitHub Pages 하위 경로 배포에 필요합니다.
- `main` 브랜치에 푸시하면 GitHub Pages가 자동으로 빌드하고 배포합니다.

## 작업 원칙

- Maxroll 같은 공략 허브 느낌을 참고하되, 레이아웃과 문구는 달빛여운 사이트에 맞게 독자적으로 구성합니다.
- 와우 자료실, 애드온, 클래스 가이드처럼 반복 접근하는 정보는 홈에서 빠르게 진입할 수 있게 둡니다.
- 긴 프로필 문자열과 표는 모바일에서 레이아웃을 깨지 않도록 처리합니다.
- 새로 만든 파일은 작업 후 `git add`까지 진행합니다.
- 불필요한 빌드 결과물, 캐시, 임시 파일은 커밋하지 않습니다.
