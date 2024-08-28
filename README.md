#FE 프로젝트
# 프로젝트 개요
HTML, CSS 이용하여 레이아웃 디자인하기
JavaScript 이용하여 기능 구현하기

# 파일 구조
├── index.html               # 메인 HTML 파일  
├── project.css              # 스타일링을 위한 메인 CSS 파일  
├── Group.png            # 로고 이미지  
├── menu.svg             # 모바일 보기용 메뉴 아이콘  
├── img_cat_png.png      # 헤더에 사용된 고양이 이미지  
├── ...                  # 기타 이미지들  
└── readMe              # 프로젝트 설명 파일  

# 기능
1. 스크롤 시 상단바(헤더) 상단 고정
2. 스크롤 탑 버튼 구현
3. 구독하기 모달창 구현
4. 모바일에서 레이아웃 변경
5. 모바일 메뉴 창 열기, 닫기

# 기능 세부 설명
1. 스크롤 시 상단바 (헤더) 상단 고정
   - 처음에는 고정된 상태가 아님, 스크롤 시 상단 고정  
     -> 상단바가 보이지 않을 때 헤더 고정   
     -> 스크롤 이벤트 -> ( 스크롤Y > 상단바 높이 ) 일 때 상단바를 상단에 고정  
 
2. 스크롤 탑 버튼
   - 스크롤시 스크롤탑 버튼 나타남  
     -> 최상단에서 스크롤 탑 버튼이 안 보임  
     -> 스크롤탑 버튼 숨김 -> 스크롤 이벤트 발생 -> (스크롤Y > 0) 일 때 스크롤 버튼에 보이는 속성 추가
   - 스크롤탑 버튼은 푸터 아래로 내려가지 않음  
     -> 버튼 높이를 푸터 높이보다 높게 지정
   - 버튼은 누르면 스크롤이 최상단으로 부드럽게 올라감  
     -> scrollTo 사용하여 최상단, 부드럽게 올라가도록 설정

3. 구독하기 모달창 구현
   - 이메일 입력 후 Subscribe 버튼 클릭시 이메일 유효성 검사,모달창 나타남  
     모달창 안 보이게 설정 -> Subscribe 버튼 클릭-> 정규표현식과 입력값 비교하여 틀리면 alert 창 -> 맞으면 모달창 보이게 변경
   - <OK! I love HODU> 버튼 클릭시 폼 제출, 모달창 닫힘

4. 모바일에서 레이아웃 변경
   섹션별로 @media (max-width: 375px) 이용하여 레이아웃 설정
   *안드로이드는 360 X 740px  iOS는 375 X 812px, 더 큰 ios를 경계로 설정

5. 모바일 메뉴 창 열기 닫기
   - 메뉴 아이콘 클릭시 메뉴창 생김
     흰색 배경과 메뉴창 숨김 -> 아이콘 클릭 -> 흰색 배경과 메뉴창 보임
   - 화살표 클릭시 메뉴창 없어짐


# 실행화면
|            | 웹                                                                                 | 모바일                      |
|------------|------------------------------------------------------------------------------------|---------------------------------------------|
| **전체화면** | <img src="./실행화면/웹스크린샷.png"/>                                           | <img src="./실행화면/모바일스샷.png" />  
| **기능**   | **웹 모달**<br><br> <img src="./실행화면/웹모달(이메일성공).png"/>                    | **모바일 모달**<br><br> <img src="./실행화면/모바일모달.png"/>              |
|            | **웹 이메일 실패시 alert**<br><br> <img src="./실행화면/웹alert(이메일실패).png"/>    |**모바일 메뉴창**<br><br> <img src="./실행화면/모바일메뉴.png"/>  
     

# 프로젝트 후기
프로젝트를 진행하면서 배웠던 개념을 체화하고 부족한 부분을 공부할 수 있어 유익한 시간이었습니다.
또 직접 페이지를 만들어가는 것이 신기하고 재미있었습니다.

아쉬운 점은 초반에 큰 틀을 보지 못하고 생각나는 대로 코드를 작성하다 보니, 전체적인 코드가 체계적이지 못했다는 것입니다. 
수정을 거듭하다 이 문제를 느끼고 앞으로는 더 효율적이고 정돈된 방식으로 코드를 작성해야겠다는 생각을 하였습니다.

처음에는 낯설고 어려워 보였던 것들이 이제는 익숙해지고, 문제를 해결하는 시간이 짧아지며 성장해가는 것을 느낄 수 있었습니다.
아직 배울 것이 더 많지만, 이번 경험을 바탕으로 자신감을 갖고 배워갈 수 있을 것 같습니다.
