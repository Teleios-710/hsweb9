# 9주차 · CSS3 고급 활용

Flexbox, Grid, 반응형 웹 디자인 기초

- 과목: 한신대학교 웹프로그래밍 (AS006-E)
- 주차 강의안: https://hs-web.dreamitbiz.com/weeks/9

## 여는 방법

1. 압축을 풉니다.
2. VS Code 에서 **폴더째로** 엽니다 (파일 → 폴더 열기).
3. `.html` 파일을 더블클릭하면 브라우저에서 바로 열립니다.
   VS Code 라면 Live Server 확장을 쓰는 편이 편합니다 — 저장하면 화면이 바로 바뀝니다.
4. 고쳐 보고, 저장하고, 브라우저를 새로고침(F5)하세요.

- `.css` 파일은 **속성 참고**입니다. 그 자체로는 화면이 안 뜹니다 — 선택자 안에 넣어 쓰세요.

**고쳐 보라고 드리는 파일입니다.** 망가뜨려도 괜찮습니다 — 다시 받으면 됩니다.

## 학습 목표

- Flexbox의 주축·교차축 개념을 이해하고 정렬 속성을 정확히 쓸 수 있다.
- Grid로 2차원 격자를 만들고 minmax·auto-fit을 활용할 수 있다.
- 미디어쿼리로 화면 폭에 따라 배치를 바꿀 수 있다.
- 미디어쿼리가 뒤 규칙에 덮여 죽는 문제를 진단하고 고칠 수 있다.
- CSS 변수로 색과 여백을 한 곳에서 관리할 수 있다.

## 이번 주 낱말

flex · justify-content · align-items · gap · grid · minmax · auto-fit · 미디어쿼리 · 모바일 우선 · CSS 변수

## 담긴 파일

### examples/ — 강의안에 나온 예제 25개

- `examples/01.html` — 켜는 곳은 자식이 아니라 부모입니다
- `examples/02.html` — flex container 속성
- `examples/03.html` — 완벽한 가운데 정렬 — 세 줄이면 끝
- `examples/04.html` — flex item 속성
- `examples/05.html` — ⚠ 기본값 nowrap의 함정
- `examples/06.html` — ① 헤더 — 로고 왼쪽, 메뉴 오른쪽
- `examples/07.html` — ① 헤더 — CSS
- `examples/08.html` — ② 미디어 오브젝트 — 이미지 옆에 글
- `examples/09.html` — ③ 푸터를 화면 아래에 붙이기 (내용이 짧아도)
- `examples/10.html` — Grid 켜기
- `examples/11.css` — fr은 "fraction(조각)"입니다
- `examples/12.css` — 실무에서 반드시 알아야 할 함정
- `examples/13.html` — 미디어쿼리 없는 반응형 격자
- `examples/14.html` — span과 grid-template-areas
- `examples/15.html` — viewport 메타 태그
- `examples/16.html` — 화면 조건에 따라 다른 규칙
- `examples/17.html` — 두 가지 방향
- `examples/18.html` — 모바일 규칙이 죽는 순간
- `examples/19.html` — 이미지 반응형의 기본
- `examples/20.html` — 표는 감싸서 스크롤시킵니다
- `examples/21.html` — 표 — CSS
- `examples/22.html` — 한국어 + 긴 URL
- `examples/23.html` — 좌우 여백을 섹션마다 하드코딩하지 않기
- `examples/24.html` — 정의하고 꺼내 쓰기
- `examples/25.html` — 기본값과 지역 변수

### lab/ — 실습 7개

- `lab/lab1.html` — 실습 1 · 기본
- `lab/lab2.html` — 실습 2 · 기본
- `lab/lab3.html` — 실습 3 · 심화
- `lab/lab4.html` — 실습 4 · 기본
- `lab/lab5.html` — 실습 5 · 응용
- `lab/lab6.html` — 실습 6 · 심화
- `lab/lab7.html` — 실습 7 · 기본

문제와 힌트는 각 실습 파일 맨 위 주석에 그대로 적어 두었습니다.
모범답안은 `lab/answer/` 에 있습니다. **먼저 스스로 해 본 뒤에** 열어 보세요.

## 다 만들었으면

실습 결과를 패들릿에 올려 자랑해 주세요.
주차 강의안 페이지 **맨 위**의 [9주차 실습 자랑하기] 단추로 들어갑니다.

> ⚠ 패들릿은 **서로 보고 배우는 자랑·질문용**입니다. 성적과는 관계가 없습니다.
> 성적에 들어가는 **실습 과제는 학교 LMS에 제출**합니다 — https://lms.hs.ac.kr/

- 실습 결과(화면 캡처) → 「9주차 실습 제출」 칸
- 막히거나 안 되는 것 → 「9주차 질문·막힌 곳」 칸

https://padlet.com/dreamitbiz/hs2605
