# WePLi-Resources (originals only)

이 레포는 WePLi 브랜드의 편집 원본을 보관하는 저장소입니다.
실행 에셋은 각 앱 레포에 포함해서 관리합니다.

## 운영 규칙

- `originals/` 디렉터리에만 원본 저장 (산출물 업로드 금지)
- 변경 시 `meta/assets.manifest.json` 업데이트
- PR에는 변경 전후 미리보기 이미지 첨부 권장

## 버전 전략

- 태그는 문서 기준으로만 사용 (vYYYYMMDD 형식을 권장)
- 앱에서는 태그를 직접 참조하지 않고 변환된 산출물을 커밋

## 디렉터리 구조

```
WePLi-Resources/
├─ README.md
├─ .gitignore
├─ .gitattributes               # Git 속성 설정
├─ .github/
│  ├─ CODEOWNERS
│  └─ pull_request_template.md
├─ meta/
│  ├─ BRAND_GUIDE.md            # 로고 사용 규칙, 금지사항
│  ├─ COLORS.json               # 팔레트 정의
│  ├─ LICENSES.md               # 외부 리소스 출처와 라이선스
│  └─ assets.manifest.json      # 원본과 소비처 매핑 메타데이터
└─ originals/
   ├─ app-icons/                # 앱 아이콘 원본
   ├─ bots/
   │  └─ backup-process/        # 백업프로세스 봇 프로필
   ├─ brand/                    # 로고, 워드마크, 심볼
   ├─ ui/                       # 일러스트, 스티커, 아이콘 세트
   ├─ marketing/                # 배너, 썸네일, 포스터 원본
   └─ fonts/                    # 커스텀 폰트 및 라이선스
```

## 파일 관리 정책

이 레포는 다른 레포지토리에서 리소스를 직접 참조할 수 있도록 이미지 파일을 일반 Git으로 관리합니다.
대용량 원본 파일(PSD, AI 등)은 필요시 별도 관리를 고려하세요.

## 기여 가이드

1. 원본 파일은 `originals/` 디렉터리에만 업로드
2. `meta/assets.manifest.json` 업데이트 필수
3. 브랜드 가이드 준수 (`meta/BRAND_GUIDE.md` 참조)
4. 외부 리소스 사용 시 라이선스 명시 (`meta/LICENSES.md`)

## 관련 레포지토리

- [WePLi-Android](https://github.com/WePLi-Team/WePLi-Android)
- [WePLi-iOS](https://github.com/WePLi-Team/WePLi-iOS)
- [WePLi-Backup](https://github.com/WePLi-Team/WePLi-Backup)
- [WePLi-Docs](https://github.com/WePLi-Team/WePLi-Docs)