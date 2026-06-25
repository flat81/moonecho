---
layout: default
title: 홈
---

<section class="hero" style="background-image: linear-gradient(90deg, rgba(8, 10, 16, .94), rgba(8, 10, 16, .58) 42%, rgba(8, 10, 16, .08)), url('{{ "/assets/images/game-room-hero.png" | relative_url }}');">
  <div class="hero__inner">
    <p class="eyebrow">달빛여운 Game Log</p>
    <h1>밤에 쌓는 플레이 기록</h1>
    <p class="hero__lead">엔딩을 본 게임, 아직 붙잡고 있는 게임, 빌드와 공략 사이에서 남긴 생각들을 차곡차곡 정리합니다.</p>
    <div class="hero__actions">
      <a class="button button--primary" href="#posts">최근 글</a>
      <a class="button button--ghost" href="{{ "/about/" | relative_url }}">블로그 소개</a>
    </div>
  </div>
</section>

<section class="section section--tight" aria-labelledby="focus-title">
  <div class="section__header">
    <p class="eyebrow">Categories</p>
    <h2 id="focus-title">읽는 방향</h2>
  </div>
  <div class="focus-grid">
    <article class="focus-card">
      <span class="focus-card__mark">01</span>
      <h3>리뷰</h3>
      <p>플레이 후 남는 감정, 전투의 손맛, 세계의 밀도, 엔딩 이후의 여운을 기록합니다.</p>
    </article>
    <article class="focus-card">
      <span class="focus-card__mark">02</span>
      <h3>플레이 로그</h3>
      <p>오늘 어디까지 갔는지, 어떤 선택을 했는지, 실패와 발견을 짧게 남깁니다.</p>
    </article>
    <article class="focus-card">
      <span class="focus-card__mark">03</span>
      <h3>빌드 노트</h3>
      <p>캐릭터 세팅, 장비 조합, 루트, 반복 플레이에서 검증한 팁을 정리합니다.</p>
    </article>
  </div>
</section>

<section class="section" id="posts" aria-labelledby="posts-title">
  <div class="section__header section__header--split">
    <div>
      <p class="eyebrow">Latest Posts</p>
      <h2 id="posts-title">최근 글</h2>
    </div>
    <a class="text-link" href="{{ "/feed.xml" | relative_url }}">RSS</a>
  </div>

  <div class="post-list">
    {% for post in site.posts %}
      <article class="post-card">
        <div class="post-card__meta">
          <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%Y.%m.%d" }}</time>
          {% if post.categories.size > 0 %}
            <span>{{ post.categories | first }}</span>
          {% endif %}
        </div>
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p>{{ post.excerpt | strip_html | truncate: 110 }}</p>
        {% if post.tags.size > 0 %}
          <div class="tag-row">
            {% for tag in post.tags limit: 3 %}
              <span>{{ tag }}</span>
            {% endfor %}
          </div>
        {% endif %}
      </article>
    {% endfor %}
  </div>
</section>
