# my-resume
A resume written in Markdown, including my skills, projects, and learning goals.<br>
Markdown 기반으로 제가 학습한 내용들을 이력서 형식으로 README파일에 작성한 레포지토리입니다.

![header](https://capsule-render.vercel.app/api?type=waving&color=auto&height=300&section=header&text=이력서:-nl-홍정안&fontAlign=10&fontSize=50)

---

> ## 인적사항

<table>
  <tr>
    <td rowspan="5" width="180" align="center">
      <img src="https://github.com/user-attachments/assets/f89143ae-fa55-4ddc-a9fa-3b84990b4f7d" width="150" style="border-radius: 8px;">
    </td>
    <td><strong>항목</strong></td>
    <td><strong>내용</strong></td>
  </tr>
  <tr>
    <td>이름</td>
    <td>홍정안</td>
  </tr>
  <tr>
    <td>전공</td>
    <td>컴퓨터공학과</td>
  </tr>
  <tr>
    <td>이메일</td>
    <td>wjddks327@gmail.com</td>
  </tr>
  <tr>
    <td>GitHub</td>
    <td><a href="https://github.com/jeongan327">https://github.com/jeongan327</a></td>
  </tr>
</table>

---

> ## 기술 스택

- #### < Programming Languages >

  ![Java](https://img.shields.io/badge/Java-007396?style=flat&logo=openjdk&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white) ![C](https://img.shields.io/badge/C-A8B9CC?style=flat&logo=c&logoColor=white) ![C#](https://img.shields.io/badge/C%23-512BD4?style=flat&logo=csharp&logoColor=white)

- #### < Frameworks / Libraries >
  ![Spring](https://img.shields.io/badge/SpringBoot-6DB33F?style=flat&logo=springboot&logoColor=white) ![ROS](https://img.shields.io/badge/ROS-22314E?style=flat&logo=ros&logoColor=white) ![Unity](https://img.shields.io/badge/Unity-000000?style=flat&logo=unity&logoColor=white) 

- #### < Tools & Environment >
  ![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white) ![VS Code](https://img.shields.io/badge/VSCode-007ACC?style=flat&logo=visualstudiocode&logoColor=white)

---

> ## 수업 기반 프로젝트 및 실습 경험

1. **News Curation Web Project**(문제해결 프로그래밍)
  - 사용기술: Spring-boot, python, mysql
  - 기간 : 2025.03.19 ~ 2025. 06.13
  - 프로젝트 내용

      기존 IT 뉴스 플랫폼이 기사 양이 많고 접하기 쉽지만,
      사용자의 선호도 기반으로 뉴스를 추천하거나 뉴스를 구분하는 카테고리의 범위가 너무 광범위해 쉽게 원하는 정보를 찾기 어렵다는 문제를 발견하였습니다.  
      이를 해결하기 위해 `newsapi.org`에서 IT 뉴스 데이터를 수집한 뒤, 
      명사 기반으로 키워드를 구분해 이를 기반으로 AI/HW/DATA/SECURITY 카테고리로 매핑 및 인기 뉴스 추천 기능을 제공합니다.

      또한, 한 기사에서 카테고리 외에 명사 기반 많은 키워드를 얻기 때문에
      사용자가 조회한 뉴스의 키워드를 기반으로 관심 기사 내용을 추측하여, 마이페이지에서 개인화된 뉴스 추천이 이루어지도록 구현하였습니다.

      **제가 담당한 주요 역할은 사용자 인증 및 사용자 관리 기능 구현입니다.**
      > - JWT 기반 로그인 및 토큰 발급/갱신 기능 구현
      > - OAuth2 로그인 설정 및 사용자 정보 처리 로직 개발
      > - Spring Security를 활용한 접근 제어 및 인증 필터 구현
      > - 사용자 회원가입, 정보 조회/수정 등 User API 개발
      > - MySQL과 연동하여 사용자 계정 및 관심 키워드 데이터 저장 구조 설계

      이를 통해 JWT. OAuth2, Spring Security의 인증/인가 구조를 직접 구성하여 JWT와 Security에 대해 많이 이해할 수 있었습니다.
      JWT는 단순한 문자열 토큰이 아니라, Header/Payload/Signature 구조로 이루어져 있고,
      보안에 취약점을 드러내지 않기 위해 Access/Refresh 토큰을 분리해 관리한다는 것,
      그리고 서버가 클라이언트이 Access토큰을 검증해 인증을 완료하는 전체 흐름을 이해하게 되었습니다.

      또한, Spring Security의 인증 절차가 단순 설정이 아닌 여러 개의 Security Filter가 연결되어 요청을 처리한다는 점을 알게 되었습니다.
      즉, JWT 기반 인증 요청이 들어왔을 때, JwtAuthenticationFilter가 Authorization 헤더를 검사하고 토큰의 유효성을 판단하고,
      유효한 토큰이라면 SecurityContextHolder에 Authentication객체를 생성해 저장하고 이를 통해 컨트롤러에서 인증된 사용자로 역할을 수행합니다.
      제가 이 프로젝트를 진행하지 않았을 땐, 이후에 당연히 토큰 정보를 저장해 토큰 만료 시간을 기준으로 동작수행여부를 정할 줄 알았는데, 이를 매 요청마다 수행한다는 것을 알게되었습니다.


2. **Unity 3D Endless Runner Game Development**(컴퓨터 그래픽스)
  - 사용기술: Unity3D
  - 기간 : 2025.09.01 ~ 2025. 11.13
  - 프로젝트 내용

      Unity 엔진을 활용하여 3D Endless Runner 형태의 게임을 개발하였습니다.
      방향 전환, 점프·슬라이딩 같은 캐릭터 이동 제어와 맵 타일 자동 생성, 장애물 스폰 로직 등
      런게임의 핵심 구조를 직접 구현하며 게임 로직의 전체 흐름을 이해했습니다.

      플레이어는 3개의 레인을 기반으로 좌·우 이동을 수행하며,
      점프 및 슬라이딩 애니메이션과 충돌 판정을 구현하여 실제 게임과 유사한 조작감을 구현했습니다.
      또한 점수 및 맵의 경우에는, 플레이어가 전진할 때 z값을 기준으로 점수 계산 및 새로운 타일을 생성하고,
      뒤에 보이지 않는 타일은 삭제하는 방식으로 런타임 맵을 동적으로 유지하는 구조를 구현하였습니다.

      장애물은 스폰 지점에서 일정 확률로 랜덤 생성되며,
      충돌 시 게임 오버 또는 특정 이벤트가 발생하도록 이벤트 기반 구조로 설계했습니다.

      이를 통해 Unity의 Update/FixedUpdate 흐름, Rigidbody 기반 물리 처리,
      Prefab을 이용한 객체 재사용, 그리고 코루틴을 통한 비동기 타일 생성 등
      게임 개발에서 활용되는 핵심 개념을 실습을 통해 깊이 이해할 수 있었습니다.

3. **시스템 프로그래밍 실습**
  - 사용기술: C
  - 기간 : 2025.09.01 ~ 2025. 11.13
  - 프로젝트 내용

    시스템 프로그래밍 수업을 통해  
    네트워크 소켓 통신, 멀티프로세스 구조, 멀티스레드 구조, 그리고 공유 메모리를 포함한 IPC 기법을 학습하였습니다.

    학습한 내용을 기반으로  
    다른 컴퓨터와 데이터를 주고받는 소켓 통신 프로그램을 작성하고,  
    멀티프로세스 기반 서버 구조 및 IPC를 활용한 데이터 교환 프로그램을 실습하였습니다.

    이를 통해 서버-클라이언트 구조에서 서버가 클라이언트 요청마다 1:1 통신 세션을 어떤 식으로 구성하는지 직접 실습하며 모호했던 부분을 명확히 이해할 수 있엇고,
    특히 IPv4와 IPv6를 같이 사용하고 있는 형태가 그냥 IPv6로 바뀌어가는 과정으로만 생각하였는데,
    `htonl()`, `htons()`, `ntohl()`, `ntohs()` 같은 바이트 오더 변환 함수가 필수적으로 사용된다는 점을 학습하며
    다양한 주소 체계를 하나의 통합된 네트워크 표현으로 다루는 과정의 중요성을 실습을 통해 명확히 체감할 수 있었습니다.

    멀티프로세스 환경에서 공유 메모리를 이용한 데이터 교환 실습을 수행하면서  
    프로세스 간 메모리 공간이 완전히 분리되어 있다는 점과,  
    공유 메모리를 통해 이를 안전하게 연결하는 구조를 실제 코드로 구현하며 깊이 이해할 수 있었습니다.
    
---

> ## 학습 목표
  어린시절부터 컴퓨터를 많이 접하고 사용하면서, 컴퓨터에서 당연시하게 사용되는 부팅, 통신, 인터넷 등 다양한 기능이 실제로 어떻게 동작하는지 많은 궁금증이 있었습니다.
  이러한 호기심을 바탕으로 여러 분야의 이론과 기술을 학습해왔으며, 앞으로는 단순한 개념 이해를 넘어 실제 구현 방식까지 깊이 있게 탐구하고자 합니다.
  특히 각 기술의 동작원리 및 여러 프로그램의 설계 방식을 이해하여, 설계된 프로그램을 구현할 때 상황에 가장 적합하고 효율적인 방식을 선택할 수 있는 수준의 개발자로 성장하는 것이 목표입니다.
  또한 이렇게 어느정도 수준의 실력을 갖췄을 때, 코드를 분석해 오픈소스 소프트웨어 역시 잘 활용하여 프로그램을 효율적이고 안정적으로 프로그램을 설계/구현할 수 있는 개발자가 되고 싶습니다.
