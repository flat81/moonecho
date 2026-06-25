---
layout: default
title: 홈
---

<section class="hero hub-hero" style="background-image: linear-gradient(90deg, rgba(7, 9, 14, .96), rgba(7, 9, 14, .68) 46%, rgba(7, 9, 14, .2)), url('{{ "/assets/images/game-room-hero.png" | relative_url }}');">
  <div class="hero__inner hub-hero__inner">
    <p class="eyebrow">게임 스트리머 달빛여운</p>
    <h1>와우 자료실과 클래스 가이드를 한곳에</h1>
    <p class="hero__lead">방송에서 자주 묻는 설정, 애드온, UI 프로필, 클래스별 메모를 빠르게 찾을 수 있도록 정리하는 달빛여운의 게임 허브입니다.</p>
    <div class="hero__actions">
      <a class="button button--primary" href="{{ "/wow/" | relative_url }}">와우 자료실</a>
      <a class="button button--ghost" href="{{ "/classes/" | relative_url }}">클래스 가이드</a>
    </div>
  </div>
</section>

<section class="section section--tight" aria-labelledby="games-title">
  <div class="section__header section__header--split">
    <div>
      <p class="eyebrow">Game Hub</p>
      <h2 id="games-title">현재 운영 중인 자료</h2>
    </div>
    <a class="text-link" href="{{ "/wow/" | relative_url }}">전체 자료 보기</a>
  </div>

  <div class="hub-grid">
    <a class="hub-card hub-card--primary" href="{{ "/wow/" | relative_url }}">
      <span class="hub-card__label">World of Warcraft</span>
      <h3>월드 오브 워크래프트 - 한밤</h3>
      <p>제작의뢰, 편집 모드 문자열, 애드온 목록, 폰트 다운로드를 모아둔 메인 자료실입니다.</p>
      <span class="hub-card__cta">자료실 열기</span>
    </a>
    <a class="hub-card" href="{{ "/classes/" | relative_url }}">
      <span class="hub-card__label">Class Guides</span>
      <h3>클래스별 가이드</h3>
      <p>조화 드루이드, 냉기 마법사, 주술사, 사제, 성기사, 전사 등 직업별 메모를 정리합니다.</p>
      <span class="hub-card__cta">가이드 보기</span>
    </a>
    <a class="hub-card" href="{{ "/wow/#addons" | relative_url }}">
      <span class="hub-card__label">Addons</span>
      <h3>애드온 설정</h3>
      <p>방송 화면과 플레이 환경에 쓰는 애드온, 명령어, 프로필 링크를 빠르게 확인합니다.</p>
      <span class="hub-card__cta">목록 확인</span>
    </a>
  </div>
</section>

<section class="section section--tight" aria-labelledby="quick-title">
  <div class="section__header">
    <p class="eyebrow">Quick Access</p>
    <h2 id="quick-title">자주 찾는 항목</h2>
  </div>

  <div class="guide-grid">
    <a class="guide-card" href="{{ "/wow/#crafting" | relative_url }}">
      <span>제작</span>
      <h3>제작의뢰 캐릭터</h3>
      <p>전문기술별 담당 캐릭터와 제작 가능 부위를 확인합니다.</p>
    </a>
    <a class="guide-card" href="{{ "/wow/#edit-mode" | relative_url }}">
      <span>UI</span>
      <h3>편집 모드 프로필</h3>
      <p>와우 편집 모드에서 붙여넣을 프로필 문자열을 보관합니다.</p>
    </a>
    <a class="guide-card" href="{{ "/wow/#details" | relative_url }}">
      <span>Details</span>
      <h3>Details 프로필</h3>
      <p>미터기 프로필과 설정 문자열을 따로 정리합니다.</p>
    </a>
    <a class="guide-card" href="{{ "/wow/#wow-font" | relative_url }}">
      <span>Download</span>
      <h3>와우 폰트</h3>
      <p>Fonts 폴더에 넣어 사용할 압축 파일을 내려받습니다.</p>
    </a>
  </div>
</section>

<section class="section" aria-labelledby="roadmap-title">
  <div class="section__header">
    <p class="eyebrow">Roadmap</p>
    <h2 id="roadmap-title">초기 업데이트 방향</h2>
  </div>

  <div class="update-list">
    <article>
      <span>01</span>
      <h3>와우 자료실 정리</h3>
      <p>Notion에 있던 애드온, UI, 다운로드 자료를 사이트 페이지로 이전합니다.</p>
    </article>
    <article>
      <span>02</span>
      <h3>클래스별 가이드 확장</h3>
      <p>직업별 세팅, 특성, 애드온 프로필, 참고 링크를 단계적으로 채웁니다.</p>
    </article>
    <article>
      <span>03</span>
      <h3>방송용 빠른 링크</h3>
      <p>시청자가 채팅에서 자주 묻는 자료를 첫 화면에서 바로 접근하게 만듭니다.</p>
    </article>
  </div>
</section>
