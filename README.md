# IP Location Service

Cloudflare Pages를 사용한 간단한 IP 주소 확인 서비스

## 설치

```bash
npm install
```

## 개발 환경 실행

```bash
npm run dev
```

로컬에서 http://localhost:8000 에 접속하여 확인할 수 있습니다.

## 배포

### 방법 1: Wrangler CLI 사용
```bash
npm run deploy
```

### 방법 2: Git 연동 (권장)
1. GitHub에 코드를 push
2. Cloudflare Dashboard에서 Pages 프로젝트 생성
3. GitHub 저장소 연결
4. 빌드 설정: 빌드 명령어 없음, 출력 디렉토리 `public`
5. 자동 배포 설정 완료

### 방법 3: 드래그 앤 드롭
Cloudflare Pages Dashboard에서 `public` 폴더를 직접 드래그하여 배포

## 프로젝트 구조

- `public/` - 정적 파일 (HTML, CSS, JS)
  - Cloudflare의 공개 API를 사용하여 IP 정보 가져오기
  - 서버사이드 코드 없이 순수 클라이언트 사이드로 동작

## 사용 방법

배포 후 제공되는 URL에 접속하면 자동으로 접속한 사용자의 IP 주소를 표시합니다.
