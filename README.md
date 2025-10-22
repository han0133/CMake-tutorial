# CMake Tutorial Study Notes

This repository documents my journey studying **CMake** through the official tutorial.  
CMake의 기본 개념부터 고급 기능까지 직접 실습한 학습 기록을 담고 있습니다.

---

## 📘 About CMake

CMake는 다양한 플랫폼과 컴파일러를 지원하는 **크로스 플랫폼 빌드 시스템 생성 도구**입니다.  
CMake를 사용하면 프로젝트의 빌드 방식을 코드로 정의하고, Makefile, Visual Studio, Ninja 등 다양한 빌드 스크립트를 자동으로 생성할 수 있습니다.

---

## 🧠 Study Log

### 1️⃣ Getting Started
- 공식 튜토리얼 Step 1 따라 하기  
  [CMake Official Tutorial](https://cmake.org/cmake/help/latest/guide/tutorial/index.html)
- 기본 `CMakeLists.txt` 작성  
- 빌드 디렉토리 분리(`build/` 생성 후 `cmake .. && make` 실행)  
- **느낀점:** Makefile을 직접 작성할 때보다 훨씬 구조적이고 유지 보수가 용이함

---

### 2️⃣ Add a Library
- `add_library()`와 `target_link_libraries()` 학습  
- 라이브러리 생성 후 실행 파일에 연결 실습  
- **실수:** target 이름 오타로 링크 에러 발생 → 터미널 로그를 꼼꼼히 확인하는 습관 필요

---

### 3️⃣ Usage Requirements
- `target_include_directories()` 명령의  
  **INTERFACE**, **PUBLIC**, **PRIVATE** 차이를 실습으로 이해  
- 빌드 스코프에 따라 include 경로가 달라지는 점 체험

---

### 4️⃣ Adding Testing
- `enable_testing()`, `add_test()` 실습으로  
  자동 테스트 환경 구축  
- 작은 단위 테스트를 정의하고 `ctest` 명령으로 결과 확인

---

### 5️⃣ Installing
- `install()` 명령으로 실행 파일과 헤더 설치 경로 지정  
- `make install` 동작 확인  
- 시스템 전역 설치 `/usr/local` 대신 로컬 디렉토리 옵션 사용해 안전하게 실습

---

### 6️⃣ Packaging with CPack
- `CPack`을 사용해 `.tar.gz` 또는 `.zip` 형태 패키지 자동 생성  
- 간단한 배포 형식 만들기 성공  
- **느낀점:** 배포 자동화의 중요성을 체감

---

## 🚀 What I Learned

- CMake 기본 빌드 플로우와 주요 명령 (`add_executable`, `add_library`, `target_link_libraries` 등)  
- INTERFACE / PUBLIC / PRIVATE 접근 지정자의 차이  
- 빌드 디렉토리 분리 및 오류 정리 습관  
- 테스트 및 설치 자동화의 핵심 구조  
- 플랫폼 독립적인 빌드 환경 구성 방법  

---

## 🔧 Next Steps

- 개인 프로젝트에 CMake 적용  
- 고급 기능 (변수, 조건문, find_package 등) 실습  
- Modern CMake 스타일 학습 (`target_*` 중심)  
- 공식 문서 업데이트 시 학습 내용 추가 기록  

---

## 📚 References

- [CMake Official Tutorial](https://cmake.org/cmake/help/latest/guide/tutorial/index.html)  
- [CMake Documentation](https://cmake.org/documentation/)  
- [Kitware GitLab - CMake Source](https://gitlab.kitware.com/cmake/cmake)

---

## 👩‍💻 Author

- **Name:** han0133
- **GitHub:** [github.com/han0133](https://github.com/han0133)  
- **Email:** soyoungahn2706@gmail.com

---

_Always learning, always building._


