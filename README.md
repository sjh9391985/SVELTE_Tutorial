# SVELTE_Tutorial

### 특징
- VIRTUAL DOM이 존재하지 않음

### 세팅방법
1. npx degit sveltejs/template svelte-tutorial
--> git svelte 주소의 내용들이 지정 디렉토리에 복사됩니다.
2. cd my svelte-tutorial
3. npm install
4. npm run dev
--> local 주소의 port 5000번 주소가 나옵니다.
5. VSCode 사용시 Svelte for VS code 플러그인 설치 
 
### 파일 내 CSS 부여하기
- 파일 내 CSS style 은 해당 파일 내 태그에서만 적용이 됩니다.

### 외부 svelte 파일 import 받기
- 외부에서 받은 svelte 파일을 import 받고자 할 경우에 첫 글자는 대문자로 지정(react랑 동일합니다.)