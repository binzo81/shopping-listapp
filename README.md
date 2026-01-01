# 쇼핑 리스트 앱

Supabase 데이터베이스를 사용하는 간단한 쇼핑 리스트 웹 애플리케이션입니다.

## 데모
https://shopping-listapp.vercel.app

## 기능

- 쇼핑 아이템 추가
- 아이템 완료 체크
- 아이템 삭제
- 실시간 통계 (전체/완료/남음)
- Supabase 클라우드 데이터베이스 연동

## 기술 스택

- HTML/CSS/JavaScript
- Supabase (PostgreSQL 데이터베이스)
- GitHub Pages (배포)

## GitHub Pages 배포 설정

1. [Repository Settings](https://github.com/binzo81/shopping-listapp/settings/pages) 페이지로 이동
2. **Source** 섹션에서:
   - Branch: `master` 선택
   - Folder: `/ (root)` 선택
3. **Save** 버튼 클릭
4. 몇 분 후 https://binzo81.github.io/shopping-listapp/ 에서 앱 확인 가능

## 로컬 실행

1. 저장소 클론
```bash
git clone https://github.com/binzo81/shopping-listapp.git
cd shopping-listapp
```

2. `index.html` 파일을 브라우저에서 열기

## 데이터베이스 구조

**shopping_items** 테이블:
- `id`: BIGSERIAL (Primary Key)
- `text`: TEXT (아이템 이름)
- `checked`: BOOLEAN (완료 여부)
- `created_at`: TIMESTAMP (생성 시간)
