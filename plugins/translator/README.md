# translator

다국어 번역 및 국제화(i18n) 지원을 위한 스킬 모음입니다.

## 설치

```bash
claude plugin install translator@osom-plugins
```

## 스킬 목록

| 스킬 | 설명 |
|------|------|
| `/translate` | 텍스트를 다른 언어로 번역 |
| `/detect` | 텍스트의 언어 감지 |
| `/i18n` | 프로젝트 국제화 파일 관리 |

## 사용 예시

### 텍스트 번역

```bash
/translate en 안녕하세요, 반갑습니다.
/translate ko Hello, nice to meet you.
/translate ja 이 기능은 사용자 인증을 처리합니다.
```

파일 전체를 번역할 수도 있습니다:

```bash
/translate ko README.md
```

### 언어 감지

```bash
/detect 이 텍스트는 무슨 언어일까요?
/detect Bonjour, comment allez-vous?
```

### 국제화 관리

번역 상태 확인:

```bash
/i18n status
```

누락된 번역 동기화:

```bash
/i18n sync
/i18n sync ko
```

새 번역 키 추가:

```bash
/i18n add common.greeting "Hello" "안녕하세요"
```

## 지원 언어

| 코드 | 언어 |
|------|------|
| `ko` | 한국어 |
| `en` | 영어 |
| `ja` | 일본어 |
| `zh` | 중국어 (간체) |
| `zh-TW` | 중국어 (번체) |
| `es` | 스페인어 |
| `fr` | 프랑스어 |
| `de` | 독일어 |
| `pt` | 포르투갈어 |
| `ru` | 러시아어 |
| `vi` | 베트남어 |
| `th` | 태국어 |
| `ar` | 아랍어 |

그 외 언어도 지원됩니다.

## 라이선스

MIT
