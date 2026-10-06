# 통합 시스템 메뉴얼 (MkDocs)

PDF 초안(2026-10-01)을 MkDocs(Material) 사이트로 변환한 프로젝트입니다.

## 배포 방법 (GitHub Pages)

1. GitHub에서 새 저장소를 만듭니다.
2. 이 폴더의 파일을 저장소에 푸시합니다 (기본 브랜치: `main`).
3. 저장소 **Settings > Pages > Build and deployment > Source**를 **GitHub Actions**로 지정합니다.
4. `main`에 푸시하면 자동으로 빌드되어 배포됩니다. Actions 탭에서 진행 상황을 볼 수 있습니다.

## 로컬에서 미리보기

```bash
pip install -r requirements.txt
mkdocs serve        # http://127.0.0.1:8000
```

## 문서 수정

- 본문: `docs/` 아래 마크다운 파일
- 목차(좌측 메뉴): `mkdocs.yml`의 `nav`
- 이미지: `docs/assets/img/`

## 공개 범위 주의

- 공개(Public) 저장소의 Pages 사이트는 주소를 아는 누구나 볼 수 있습니다.
- `noindex` 메타 태그와 `robots.txt`를 넣어 검색엔진 노출은 막아두었지만, **접근 제한은 아닙니다.**
- 광고주 정보나 내부 화면을 추가할 때는 공개해도 되는지 먼저 확인하세요.
