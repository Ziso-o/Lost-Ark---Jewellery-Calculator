# Lost Ark 회랑 계산기

보유 보석과 회랑 티켓(노말/하드/헬/영겁)을 입력하면 획득 가능한 보석 수량을 계산해주는 도구입니다.

**URL:** http://loajew.dothome.co.kr

---

## 기능

- 보유 보석 레벨(1~9) 수량 입력
- 회랑 티켓 종류별(노말 / 하드 / 헬 / 영겁) 수량 입력
- 보석 합산 계산 및 결과 표시

## 프로젝트 구조

```
/
├── index.html          # 메인 페이지
├── favicon.png         # 파비콘
├── fonts/              # 페이퍼로지 폰트 (로컬)
│   ├── Paperlogy-Regular.woff2
│   ├── Paperlogy-SemiBold.woff2
│   └── Paperlogy-ExtraBold.woff2
├── images/             # 회랑 이미지
│   ├── normal.png
│   ├── hard.png
│   ├── hell.png
│   └── eternal.png
└── .github/
    └── workflows/
        └── deploy.yml  # Dothome FTP 자동 배포
```

## 배포

`main` 브랜치에 push 시 GitHub Actions가 Dothome FTP로 자동 배포됩니다.

필요한 GitHub Secrets:

| Secret | 값 |
|---|---|
| `FTP_HOST` | `loajew.dothome.co.kr` |
| `FTP_USERNAME` | `loajew` |
| `FTP_PASSWORD` | FTP 비밀번호 |

---

2022. ⓒ ZisoB All rights reserved.
