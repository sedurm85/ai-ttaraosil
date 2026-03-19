---
name: lecture-writing
description: AI 강의 자료를 GitBook 형식으로 작성하는 도메인 지식
version: 1.0.0
---

# 강의 자료 작성 스킬

## GitBook 마크다운 문법

### 기본 구조
```markdown
# 페이지 제목

본문 내용...

## 섹션 제목

### 하위 섹션
```

### Hint 블록
```markdown
{% hint style="info" %}
참고할 정보를 여기에 작성합니다.
{% endhint %}

{% hint style="warning" %}
주의사항을 여기에 작성합니다.
{% endhint %}

{% hint style="danger" %}
위험/금지 사항을 여기에 작성합니다.
{% endhint %}

{% hint style="success" %}
성공/완료 메시지를 여기에 작성합니다.
{% endhint %}
```

### 탭 블록
```markdown
{% tabs %}
{% tab title="Python" %}
\```python
print("Hello")
\```
{% endtab %}
{% tab title="JavaScript" %}
\```javascript
console.log("Hello")
\```
{% endtab %}
{% endtabs %}
```

### 코드 블록 with 파일명
```markdown
{% code title="example.py" %}
\```python
def hello():
    print("Hello, World!")
\```
{% endcode %}
```

## 강의 섹션 템플릿

### 챕터 README.md
```markdown
# {챕터 제목}

{챕터 개요 1-2문장}

## 학습 목표

이 챕터를 마치면 다음을 할 수 있어요:
- 목표 1
- 목표 2
- 목표 3

## 목차

| 섹션 | 내용 |
|------|------|
| [섹션1](01-section.md) | 설명 |
| [섹션2](02-section.md) | 설명 |
```

### 일반 섹션
```markdown
# {섹션 제목}

## 개요
{이 섹션에서 다루는 내용 요약}

## 본문
{핵심 내용}

### 실습
{hands-on 예제}

## 핵심 요약
- 포인트 1
- 포인트 2
- 포인트 3
```

## SUMMARY.md 형식
```markdown
# Table of contents

* [소개](README.md)

## Part 1: 기초

* [챕터 1: 제목](chapters/01-slug/README.md)
  * [섹션 1.1](chapters/01-slug/01-section.md)
  * [섹션 1.2](chapters/01-slug/02-section.md)

## Part 2: 심화

* [챕터 2: 제목](chapters/02-slug/README.md)
```
