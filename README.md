# 9등급 환산 적정 대학 찾기

5등급제 내신 성적을 9등급제로 환산하여, 2025학년도 입결 자료를 바탕으로 적정 대학을 탐색할 수 있는 웹앱입니다.

## 파일 구성

- `src/` : 화면 및 로직 소스 코드
- `src/data/` : 환산 및 입결 데이터
- `src/lib/` : 대학 추천/진단 유틸리티
- `index.html` : 앱 진입 파일
- `package.json` : 프로젝트 실행 설정
- `.env.example` : 환경변수 예시 파일

## 로컬 실행 방법

### 1) 준비
- Node.js 설치
- Git 설치

### 2) 프로젝트 내려받기
```bash
git clone https://github.com/내아이디/내저장소이름.git
cd 내저장소이름
```

### 3) 패키지 설치
```bash
npm install
```

### 4) 환경변수 파일 준비
필요한 경우 `.env.example`을 복사해서 `.env.local` 파일을 만든 뒤 값을 넣습니다.

```bash
cp .env.example .env.local
```

### 5) 개발 서버 실행
```bash
npm run dev
```

브라우저에서 보통 `http://localhost:3000` 으로 접속하면 됩니다.

## 배포용 빌드
```bash
npm run build
```

빌드가 완료되면 `dist/` 폴더가 생성됩니다.

## GitHub에 업로드하는 방법

### 방법 1. 웹사이트에서 바로 업로드
1. GitHub 로그인
2. 오른쪽 상단 `+` 클릭
3. `New repository` 선택
4. Repository name 입력
   - 예: `grade-conversion-college-finder`
5. `Public` 또는 `Private` 선택
6. `Create repository` 클릭
7. 생성된 저장소 화면에서 `uploading an existing file` 클릭
8. 이 압축파일을 풀어서 나온 **모든 파일과 폴더**를 드래그하여 업로드
   - 단, `node_modules` 폴더는 올리지 않음
   - `.env.local` 파일은 올리지 않음
9. 아래 `Commit changes` 클릭

### 방법 2. Git 프로그램으로 업로드
저장소를 만든 뒤 아래 명령어를 순서대로 실행합니다.

```bash
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/내아이디/내저장소이름.git
git push -u origin main
```

## 다른 사람과 공유하는 방법

### 저장소 전체 공유
공개 저장소라면 아래 주소만 전달하면 됩니다.
```text
https://github.com/내아이디/내저장소이름
```

### 코드 내려받기 링크 공유
저장소 화면의 초록색 `Code` 버튼 → `HTTPS` 주소 복사 후 공유합니다.

## 주의할 점
- `node_modules`는 업로드하지 않아도 됩니다.
- `.env.local`, API 키, 비밀번호 같은 민감 정보는 절대 업로드하면 안 됩니다.
- 수정 후에는 아래 명령어로 다시 반영할 수 있습니다.

```bash
git add .
git commit -m "update"
git push
```

## 추천 저장소 이름
- `grade-conversion-college-finder`
- `9grade-college-checker`
- `school-grade-conversion-app`
