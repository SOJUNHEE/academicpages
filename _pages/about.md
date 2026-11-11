---
permalink: /
layout: splash
title: "현장을 이해하고, 데이터로 물류 운영을 개선합니다."
excerpt: "3PL·풀필먼트 센터와 무역회사에서 4년 8개월 동안 겪은 운영 문제를 데이터·AI 도구로 풀고 있는 물류 운영 포트폴리오"
redirect_from:
  - /about/
  - /about.html
---

<!-- 대시보드형 홈 (2026-11-10): 헤더 카드 → 경력 KPI → 대표 프로젝트 → 경력·AX 결과 → 역량 → 연락처.
     수치와 문구는 JUNHEE_Portfolio/data/*.json(Flask 운영 사이트)과 같다. 회사별 수치는 합산하지 않는다. -->

<section class="jk-hero" aria-labelledby="jk-hero-title">
  <p class="jk-eyebrow">3PL·풀필먼트 · 물류 운영 · 데이터·자동화</p>
  <p class="jk-name">Junhee So</p>
  <h1 id="jk-hero-title">현장을 이해하고, <span>데이터로 물류 운영을 개선합니다.</span></h1>
  <p class="jk-lead">3PL·풀필먼트 센터와 무역회사에서 4년 8개월 동안 겪은 운영 문제를, AI 코딩 도구로 직접 대시보드를 만들어 풀고 있습니다. 운영 기준은 직접 정하고, 계산 결과는 자동 점검으로 확인합니다.</p>
  <ul class="jk-facts">
    <li>물류·무역 실무 <b>4년 8개월</b></li>
    <li>3PL·풀필먼트 센터 <b>3곳</b> · 수입통관 <b>1곳</b></li>
    <li>한국무역아카데미 <b>무역 AX 2기</b></li>
  </ul>
  <p class="jk-actions">
    <a class="jk-btn primary" href="{{ '/portfolio/' | relative_url }}">프로젝트 보기</a>
    <a class="jk-btn" href="{{ '/cv/' | relative_url }}">이력 보기</a>
    <a class="jk-btn" href="mailto:sojh90@naver.com">sojh90@naver.com</a>
  </p>
</section>

<section class="jk-card" aria-labelledby="jk-kpi-title">
  <header class="jk-card-head"><h2 id="jk-kpi-title">실무 경력 지표</h2><p>회사별 수치이며 서로 합산하지 않았습니다</p></header>
  <dl class="jk-kpis">
    <div><dt>물류·무역 실무 경험</dt><dd class="v">4년 8개월</dd><dd class="s">전체 경력</dd></div>
    <div><dt>월 출고 운영 경험</dt><dd class="v">50,000건+</dd><dd class="s">굿앤파트너스</dd></div>
    <div><dt>화주사 대응</dt><dd class="v">약 15개사</dd><dd class="s">굿앤파트너스</dd></div>
    <div><dt>재고 정확도</dt><dd class="v">99%</dd><dd class="s">제이아이로지스</dd></div>
    <div><dt>월 마감 소요일</dt><dd class="v">7일 → 3일</dd><dd class="s">두잇로지스</dd></div>
    <div><dt>장기 적치 보관비</dt><dd class="v">약 10% 감소</dd><dd class="s">젠미코리아</dd></div>
  </dl>
</section>

<section class="jk-card" aria-labelledby="jk-proj-title">
  <header class="jk-card-head"><h2 id="jk-proj-title">대표 프로젝트</h2><p>1번만 회사 실무이고, 2~4번은 개인·팀 프로젝트입니다</p><a class="jk-arrow" href="{{ '/portfolio/' | relative_url }}" aria-label="프로젝트 전체 보기">↗</a></header>
  <div class="jk-projects">
    {% for p in site.portfolio %}
    <article class="jk-project">
      <a class="jk-thumb{% if p.image_note %} contain{% endif %}" href="{{ p.url | relative_url }}" tabindex="-1" aria-hidden="true">{% if p.header.teaser %}<img src="{{ '/images/' | append: p.header.teaser | relative_url }}" alt="" loading="lazy" width="1600" height="1000">{% endif %}</a>
      <div class="jk-project-body">
        <p class="jk-kind">{{ p.kind }}</p>
        <h3><a href="{{ p.url | relative_url }}">{{ p.title }}</a></h3>
        <p class="jk-excerpt">{{ p.excerpt | strip_html | truncate: 150 }}</p>
        {% if p.role_short %}<p class="jk-role">{{ p.role_short }}</p>{% endif %}
        {% if p.image_note %}<p class="jk-note">{{ p.image_note }}</p>{% endif %}
      </div>
    </article>
    {% endfor %}
  </div>
</section>

<div class="jk-row">
  <section class="jk-card jk-span-2" aria-labelledby="jk-career-title">
    <header class="jk-card-head"><h2 id="jk-career-title">경력</h2><p>최근 순 · 성과는 해당 재직 기간 기준</p><a class="jk-arrow" href="{{ '/cv/' | relative_url }}" aria-label="이력 자세히 보기">↗</a></header>
    <ol class="jk-timeline">
      <li><span class="when">2024.06 — 2026.06</span><b>젠미코리아</b><span class="what">무역행정팀 · 일본 수입식품 통관 서류 · UNI-PASS · 보세창고 일정 · 사방넷 출고 데이터</span><span class="hit">장기 적치 보관비 약 10% 감소 · 프리타임 준수율 100%</span></li>
      <li><span class="when">2023.12 — 2024.05</span><b>두잇로지스</b><span class="what">물류운영부 팀장 · 신규 센터 WMS 세팅 · FCL 입출고 · 화주사별 정산</span><span class="hit">월 마감 7일 → 3일 · 보관 효율 약 28% 개선</span></li>
      <li><span class="when">2022.04 — 2023.09</span><b>제이아이로지스</b><span class="what">센터장 · 다품종 소형가전 3PL · 재고·피킹·패킹 · 단가 관리와 정산</span><span class="hit">재고 정확도 99% · 오출고율 월 1% 미만</span></li>
      <li><span class="when">2021.09 — 2022.03</span><b>굿앤파트너스</b><span class="what">메쉬코리아 김포 풀필먼트 · B2C·B2B 출고 · WMS · 월간 재고 마감</span><span class="hit">월 50,000건 이상 출고 · 약 15개 화주사</span></li>
    </ol>
  </section>
  <section class="jk-card" aria-labelledby="jk-ax-title">
    <header class="jk-card-head"><h2 id="jk-ax-title">AX 프로젝트 결과</h2><p>가상 데이터와 로컬 측정 기준</p></header>
    <ul class="jk-ax">
      <li><b>5 / 5</b><span>일부러 넣은 정산 오류를 실적 대조로 찾아냄</span><em>다품종 3PL · 가상 데이터</em></li>
      <li><b>447,538</b><span>계산 점검 항목 모두 통과</span><em>다품종 3PL · 가상 데이터 자동 점검</em></li>
      <li><b>466 → 221MB</b><span>무료 서버 강제 종료 해결 (최대 메모리)</span><em>AXPORT · Windows 로컬 재측정 · 과거 기록 215MB</em></li>
    </ul>
  </section>
</div>

<section class="jk-card" aria-labelledby="jk-skill-title">
  <header class="jk-card-head"><h2 id="jk-skill-title">핵심 역량</h2><p>실무 경험과 학습·적용 중인 역량을 구분했습니다</p></header>
  <div class="jk-skills">
    <div><b>3PL·풀필먼트 운영</b><span>입출고 관리 · B2C·B2B 출고 · 화주사 대응 · 채널별 작업계획</span></div>
    <div><b>재고·시스템 관리</b><span>WMS · DAS · Excel 전산관리 · 월간 재고 마감·실사</span></div>
    <div><b>현장 생산성·정산</b><span>인력 배치 · 생산성 데이터 · 작업 동선 개선 · 물류비 정산</span></div>
    <div><b>수입통관·업무 자동화</b><span>Invoice·B/L·P/L 검토 · UNI-PASS · 사방넷 · <em>학습·적용 중:</em> Python · AI 업무 자동화</span></div>
  </div>
</section>

<section class="jk-card jk-contact" aria-labelledby="jk-contact-title">
  <header class="jk-card-head"><h2 id="jk-contact-title">연락처</h2><p>더 나은 운영을 만드는 일, 함께 이야기하고 싶습니다</p></header>
  <p class="jk-actions">
    <a class="jk-btn primary" href="mailto:sojh90@naver.com">이메일 sojh90@naver.com</a>
    <a class="jk-btn" href="https://github.com/SOJUNHEE">GitHub</a>
    <a class="jk-btn" href="https://portfolio-sojunhee.vercel.app/">운영 중인 포트폴리오 사이트</a>
  </p>
</section>
