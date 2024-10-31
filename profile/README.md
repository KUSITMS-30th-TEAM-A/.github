# 🧑🏻‍💻👩🏻‍💻 Three-Peat's Developers

|<img src="https://github.com/inaemon.png" width="200" height="200" />|<img src="https://github.com/2unhi.png" width="200" height="200" />|<img src="https://github.com/bbbang105.png" width="200" height="200" />|<img src="https://github.com/juuuunny.png" width="200" height="200" />
|:---:|:---:|:---:|:---:|
|[박인애](https://github.com/bbbang105)|[이은학](https://github.com/Kong-E)|[한상호](https://github.com/bin-pro)|[박준형](https://github.com/bin-pro)|
|Frontend Lead|Frontend|Backend Lead|Backend|

<br>

# 🌐 System Architecture
<img width="755" alt="히트존_아키텍처" src="https://github.com/user-attachments/assets/f2a6e9b6-bea2-487d-a619-63e92315dca2">

<br><br>

# 🧱 ERD
<img width="1242" alt="히트존_ERD" src="https://github.com/user-attachments/assets/23c4f9f0-8ba9-46bd-96e5-ad4909c5c166">

<br><br>

# 📄 API Documentation
- [API 명세서 링크 📄](https://git.hitzone.store/swagger-ui/index.html#/)
- REST Docs와 Swagger를 결합하였습니다

<br>

# 🔒 Rules

## 🖥️ Frontend

### **Issue & PR**

- 이슈 템플릿 설정
    - 기능 이슈
    - 버그 이슈
- 프론트 맞춤형 PR 템플릿 설정
- `Code Review & Approve` 룰 설정
    - 상대방이 `Approve` 올린 사람이 `Merge`

### Branch

- 생성한 이슈에 따라서 브랜치 생성 `Ex) feature/#4-login`
- `feature branch` : 각 새로운 기능
- `develop branch` : 실 개발 진행
- `hotfix branch` : 배포 이후 긴급 수정
- `main branch` : 개발 최종 완료 시 merge

### **Commit Message**

- 이슈 번호와 이모지를 붙여서 커밋
- `Ex) #4 🚀feat: 로그인 기능을 추가한다`
- Body는 추가 설명 필요하면 사용

| ***작업태그*** | ***내용*** |
| --- | --- |
| **feat** | 새로운 기능 추가 / 일부 코드 추가 / 일부 코드 수정 (리팩토링과 구분)  |
| **design** | 새로운 컴포넌트 추가 / 디자인 요소 수정 |
| **fix** | 버그 수정 |
| **refactor** | 코드 리팩토링 |
| **style** | 코드 의미에 영향을 주지 않는 변경사항 (코드 포맷팅, 오타 수정, 변수명 변경, 에셋 추가) |
| **chore** | 빌드 부분 혹은 패키지 매니저 수정 사항 / 파일 이름 변경 및 위치 변경 / 파일 삭제 |
| **docs** | 문서 추가 및 수정 |
| **rename** | 패키지 혹은 폴더명, 클래스명 수정 (단독으로 시행하였을 시) |
| **remove** | 패키지 혹은 폴더, 클래스를 삭제하였을 때 (단독으로 시행하였을 시) |

### Naming

- All Camel case

### Package

```
 ├─ components
 ├─ assets
 ├─ hooks (= hoc)
 ├─ pages
 ├─ constants
 ├─ config
 ├─ styles
 ├─ services (= api)
 ├─ utils
 ├─ contexts
 ├─ App.js
 └─ index.js
```

### 상태 관리

- 다양한 상태 관리 방법들 중 ContextAPI 으로 결정함
    - import { SettingProvider } from './setting.Context';
    - import { useSettingContext } from './setting.Context';

### API 컴포넌트화

- API Type
- API Service
- custom hook

위 3가지로 관리하기로 확정함

### 기술 스택

- React
- tailwind css
- Next.js
- Vercel

### 반응형 구현 방식

- tailwind css 이용

## 🚀 Backend

### **Issue & PR**

- 템플릿 설정
- `Code Review & Approve` 룰 설정
    - 상대방이 `Approve` 올린 사람이 `Merge`

### Branch

- 생성한 이슈에 따라서 브랜치 생성 `Ex) feature/#4/login`
- `main branch` : 개발 최종 완료 시 merge
- `develop branch` : 실 개발 진행
- `feature branch` : 각 새로운 기능
- `hotfix branch` : 배포 이후 긴급 수정

### **Commit Message**

- 이슈 번호 붙여서 커밋 `Ex) #4 [feat] : 로그인 기능을 추가한다`
- Body는 추가 설명 필요하면 사용

| ***작업태그*** | ***내용*** |
| --- | --- |
| **feat** | 새로운 기능 추가 / 일부 코드 추가 / 일부 코드 수정 (리팩토링과 구분) / 디자인 요소 수정 |
| **fix** | 버그 수정 |
| **refactor** | 코드 리팩토링 |
| **style** | 코드 의미에 영향을 주지 않는 변경사항 (코드 포맷팅, 오타 수정, 변수명 변경, 에셋 추가) |
| **chore** | 빌드 부분 혹은 패키지 매니저 수정 사항 / 파일 이름 변경 및 위치 변경 / 파일 삭제 |
| **docs** | 문서 추가 및 수정 |
| **rename** | 패키지 혹은 폴더명, 클래스명 수정 (단독으로 시행하였을 시) |
| **remove** | 패키지 혹은 폴더, 클래스를 삭제하였을 때 (단독으로 시행하였을 시) |

### Naming

- **패키지명** : 한 단어 소문자 사용 `Ex) service`
- **클래스명** : 파스칼 케이스 사용 `Ex) JwtUtil`
- **메서드명** : 카멜 케이스 사용, 동사로 시작  `Ex) getUserScraps`
- **변수명** : 카멜 케이스 사용 `Ex) jwtToken`
- **상수명** : 대문자 사용 `Ex) EXPIRATION_TIME`
- **컬럼명** : 스네이크 케이스 사용 `Ex) user_id`

### Package

- global
- user
    - application
    - domain
        - entity
            - entity
            - enums
        - repository
            - ~repository
            - custom
                - ~customRepository
                - ~impl
    - dto
        - request
        - response
    - presentation
    - exception
        - ~Exception
        - ~ErrorResult
        
        …
        
- board

### API Response

```json
{
    "code": "201",
    "message": "단축 URL 변환에 성공했습니다.",
    "payload": {
        "shorten_url": "https://1-ti.me/26kCW15Algs3EF1e3kxqCu"
    },
    "is_success": true
}
```

- `code` : 성공 코드, HTTP 상태 코드와 동일함
- `message` : 성공 메세지, 커스텀 가능
- `payload` : 데이터가 들어가는 곳
- `is_success` : 성공 여부
