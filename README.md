# 달빛여운의 게임 블로그

GitHub Pages + Jekyll 기반 정적 블로그입니다.

## 배포

1. 이 저장소를 GitHub에 `moonecho.github.io` 이름으로 연결합니다.
2. 저장소 **Settings → Pages**에서 소스가 **Deploy from a branch**이고 브랜치가 `main` / `/ (root)`인지 확인합니다.
3. `main`에 푸시하면 빌드 후 `https://moonecho.github.io` 에 반영됩니다.

## 글 추가

`_posts`에 `2026-04-02-글제목.md` 형식으로 파일을 만들고, 상단에 `layout: post`, `title`, `date` 등을 적습니다.

## 로컬 미리보기 (선택)

[Ruby](https://www.ruby-lang.org/)와 Bundler가 있을 때:

```bash
bundle install
bundle exec jekyll serve
```

브라우저에서 `http://127.0.0.1:4000` 으로 확인합니다.
