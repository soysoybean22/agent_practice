# Commit Convention

## 커밋 메시지 구조

```
<type> subject

body

footer
```

---

## Type (필수)

| 타입 | 설명 |
|------|------|
| `feat` | 새로운 기능 추가 |
| `fix` | 버그 수정 |
| `docs` | 문서 수정 (README, 주석 등) |
| `style` | 코드 포맷 변경 (기능 변경 없음) |
| `refactor` | 코드 리팩토링 (기능 변경 없음) |
| `test` | 테스트 코드 추가 또는 수정 |
| `chore` | 빌드 설정, 패키지 관리 등 기타 변경 |
| `revert` | 이전 커밋 되돌리기 |

---

## 헤더 규칙 (필수)

- 타입은 반드시 `< >` 문자로 감싸서 작성합니다.
- 형식: `<type> subject`
- 예시: `<fix> 긴급 Fix`

---

## 언어 규칙 (필수)

- 커밋 메시지(subject, body, footer)는 **한글**로 작성합니다.

---

## Subject (필수)

- 50자 이내로 작성
- 명령형으로 작성 (과거형 사용 금지)
- 마침표 없이 작성
- **한글** 사용

---

## Body (선택)

- 72자 이내로 줄 바꿈
- **무엇을**, **왜** 변경했는지 설명
- Subject와 한 줄 띄어서 작성
- **한글** 사용

---

## Footer (선택)

- 관련 이슈 번호 참조: `Closes #123`, `Refs #456`
- Breaking Change 표기: `BREAKING CHANGE: <설명>`

---

## 예시

```
<feat> JWT 로그인 기능 추가

사용자 인증 방식을 세션에서 JWT 토큰 방식으로 변경.
로그인 시 access token과 refresh token을 발급한다.

Closes #42
```

```
<fix> 긴급 Fix

사용자 엔드포인트에서 null 응답 시 500 에러 발생 문제 수정.

Refs #87
```

```
<docs> README 설치 가이드 업데이트
```
