# GitHub Pages 포트폴리오 배포 가이드

## 📁 이 폴더에 포함된 파일
- `index.html` - 포트폴리오 웹페이지 (PDF 뷰어 포함)
- `Eunmin_Park_iOS_Developer_Portfolio.pdf` - 포트폴리오 PDF

---

## 🚀 배포 방법 (Step by Step)

### Step 1: GitHub 레포지토리 생성

1. GitHub.com 접속 → 로그인
2. 오른쪽 상단 `+` 클릭 → `New repository`
3. Repository name: `portfolio` (또는 원하는 이름)
4. Public 선택 (GitHub Pages 무료 사용을 위해)
5. `Create repository` 클릭

### Step 2: 파일 업로드

**방법 A: GitHub 웹에서 직접 업로드**
1. 생성된 레포지토리 페이지에서 `Add file` → `Upload files`
2. 이 폴더의 `index.html`과 `Eunmin_Park_iOS_Developer_Portfolio.pdf` 드래그 앤 드롭
3. `Commit changes` 클릭

**방법 B: Git 명령어 사용**
```bash
# 레포지토리 클론
git clone https://github.com/Minapak/portfolio.git
cd portfolio

# 파일 복사 (이 폴더의 파일들을 복사)
# index.html과 PDF 파일을 portfolio 폴더로 복사

# 커밋 & 푸시
git add .
git commit -m "Add portfolio files"
git push origin main
```

### Step 3: GitHub Pages 활성화

1. 레포지토리 페이지에서 `Settings` 탭 클릭
2. 왼쪽 메뉴에서 `Pages` 클릭
3. **Source** 섹션에서:
   - Branch: `main` 선택
   - Folder: `/ (root)` 선택
4. `Save` 클릭

### Step 4: 배포 확인 (1-2분 소요)

배포 완료 후 접속 가능한 URL:
```
https://minapak.github.io/portfolio/
```

> ⚠️ `minapak`을 본인의 GitHub username으로, `portfolio`를 레포지토리 이름으로 변경하세요.

---

## 🔗 최종 URL 예시

| 용도 | URL |
|------|-----|
| 포트폴리오 페이지 | `https://minapak.github.io/portfolio/` |
| PDF 직접 링크 | `https://minapak.github.io/portfolio/Eunmin_Park_iOS_Developer_Portfolio.pdf` |

---

## 💡 Upwork/LinkedIn에 링크 추가하기

### Upwork 프로필에 추가:
1. Upwork 프로필 → `Edit Profile`
2. Portfolio 섹션에서 `Add Project`
3. **Project URL**: `https://minapak.github.io/portfolio/`

### LinkedIn에 추가:
1. LinkedIn 프로필 → `Add profile section`
2. `Featured` 선택
3. `Add a link` → GitHub Pages URL 입력

---

## 🎨 커스터마이징 (선택사항)

### index.html 수정 포인트:

1. **Upwork 링크 변경** (현재 설정됨):
```html
<a href="https://www.upwork.com/freelancers/~0148c177b041f931fe" target="_blank">💼 Upwork</a>
```

2. **스킬 태그 수정**:
```html
<div class="skills-preview">
    <span class="skill-tag">Swift</span>
    <span class="skill-tag">SwiftUI</span>
    <!-- 원하는 스킬 추가/수정 -->
</div>
```

3. **색상 변경** (CSS에서):
```css
/* 배경 그라데이션 */
background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%);

/* 버튼 색상 */
background: linear-gradient(90deg, #3b82f6, #2563eb);
```

---

## 🔧 문제 해결

### PDF가 안 보일 때:
- 파일명이 정확히 `Eunmin_Park_iOS_Developer_Portfolio.pdf`인지 확인
- 대소문자 구분됨!

### 404 에러:
- GitHub Pages 설정에서 Branch가 `main`으로 되어있는지 확인
- 배포까지 1-2분 소요될 수 있음

### 캐시 문제:
- 브라우저 캐시 삭제 또는 시크릿 모드로 확인

---

## 📱 모바일 최적화

이 페이지는 모바일 반응형으로 제작되었습니다:
- 작은 화면에서 자동으로 레이아웃 조정
- PDF 뷰어 높이 자동 조절
- 터치 친화적 버튼 크기
