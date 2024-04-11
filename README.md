# Visual Studio code(Vscode)
* vs code 실행 시 가장 먼저 확인해야 할 것!
* 왼쪽 탐색기가 당일 작업폴더로 연결되어 있는지 확인하기!
* (위) 안되어있다면 -> 파일 -> 작업폴더닫기 후 -> 폴더열기 다시진행!
# html 시작
* git, gitHub 개념공부
* `<태그>` 웹페이지에서 의미적인 정보를 가지는 대상
## HTML5 버전 선언
* `<!doctype html>`
## HTML 구조 태그
* html : 웹의 시작과 끝, 문서 자체 의미.
* head : 웹 문서의 정보, 제목 포함
* meta : 웹 문서의 정보 기록
* title : 웹 문서의 제목 (브라우저 상단 표시)
* body : 웹 문서의 내용 (실제 대부분의 서비스가 들어가는 본문)
## 구조 태그 속성
* `lang="ko"` html 문서 언어 설정
* `charset="utf-8"` 다국어 문자열 설정
* `keywords` 사이트 검색 키워드 설정
## 속성 문법
* `<태그 속성="값" 속성="값"></태그>`
* 태그와 속성 사이 공백
* 속성과 속성 사이 공백 (속성 개수 제한 없음)
* 속성은 시작태그에만 작성하기!
## 구조태그의 'title' 작성방법
* 메인페이지 -> 사이트명
* 메인페이지 -> 사이트명 | 광고문구추가
* 서브페이지 -> 페이지명 | 사이트명
* ex) 책이름-저자명 | 서점명
* ex) 판매아이템명 | 사이트명
## h1 ~ h6 제목 태그 (block tag)
* h1~h3 태그는 meta keywords와 동일한 검색키워드로 활용된다.(대제목일수록 높음)
* h4~h6 태그는 거의 사용하지 않는다.
* h1 대제목은 사이트의 로고 및 서브페이지 제목에서 주로 사용한다.
* h 제목의 1~6레벨은 순서대로 작성해야 한다.
## 단락 p(block tag)
* 한 줄 또는 여러 줄 단락 묶을 때 사용하는 태그
* 제목(h)태그 종류와는 형제 태그 관계로 사용해야 한다. 부모-자식(x)
## 인라인태그 br, em, strong, del, s, sup, sub 
* `br` : 블록 내 줄바꿈 태그
* `em` : 블록 내 강조 태그, 주로 내용 태그(p) 등에서 자식으로 사용
* `strong` : 블록 내 경고용 강조 태그 (위와 특징 동일)
* `del` : 삭제 텍스트, 쇼핑몰의 할인 전 가격 등에 사용
* `s` : 교체 텍스트, 쇼핑몰의 할인 전 가격 등에 사용 (del 자주사용)
* `sup, sub` : 윗첨자(sup) 아래첨자(sub) 수학, 과학 등의 기호에 사용
## 인용문 처리 blockquote, q
* `blockquote (block)` : 단락 자체가 인용문에 해당할 때 사용, p태그와 부모-자식 관계로 사용해선 안된다!
* `q (inline)` : 단락(p) 내에서 일부가 인용문에 해당할 때 사용
* 공통 습성 `cite="URL"` : `blockquote`, `q` 로 인용문 처리할 경우 출처 표시 용도로 주소(URL)을 담아주는 속성
## 특수문자 태그
* `&` 시작 `;` 종료
* `&;` 가운데에 특수문자를 넣는다
* `&lt;`는 <(여는기호), `&gt;`는 >(닫는 기호)
* `&copy;`는 카피라이트
## 주소태그
* `address (block)` 는 주소, 연락처, 회사소개, 고객센터 등등을 적는 footer 영역에 사용하는 태그이다.
* inline 요소만 넣을 수 있다. (다른 블록을 자식,자손으로 넣을 수 없음)
## 수평선 태그
* `hr (block)` 블록 태그로 복잡한 html 경계를 구분하는 구분선(수평선)을 만들어준다.
* 주석과 같은 역할을 한다. (css에서는 보이지 않음)
## 컴퓨터 명령어 태그
* `code` (긴 인용문) (inline 태그) (웹강의사이트에서 주로 사용하는 태그)
* 컴퓨터가 지원하는 다양한 명령어를 화면 표시할 경우 사용
* ex ` `, 를 묶으면 css 에서 공통으로 처리하게 끔 하는 기능
## 링크 태그 a
* block, inline 특징을 모두 가진다.
* 절대경로와 상대경로를 href 속성에 작성한다.
* 상대경로는 a태그 작성 중인 파일 위치 기준으로 연결하고자 하는 목적지 파일이 (같은, 하위, 상위) 위치인지에 따라 작성한다.
* `./` 현재 위치에서 시작
* `../` 상위 폴더로 나가기 (내가 현재 있는 폴더 밖으로 나가기)
* `../a/doll.jpg` : 상위폴더로 나가서 >> a 폴더로 가서 >> doll.jpg 파일 찾기
* `./b/doll.jpg` : 현재 위치에서 >> b폴더로 가서 >> doll.jpg 파일 찾기
## 바로가기링크란?
* 단순 페이지 이동이 아닌, 특정 위치로 스크롤 이동하는 바로가기 기능
* a태그와 id를 활용하여, 해당 페이지(목적지)로 연결해주는 기능
## 바로가기 링크 제작 순서 및 주의사항
* 1. 이동 목적지에 가장 가까운 태그에 `id` 적용하기
* 2. 링크 대상에 `#id` href 속성값에 담기
* 주의사항 : #은 아이디 이동 링크에만 사용하기
* 1)바로가기 링크는 `<a href="#목적지이름">` : a태그로 목적지와 연결할 임시경로(#)를 만든다.
* 2)목적지는 `<태그 id="목적지이름">` : 태그에 id를 입력한다.
* `#`은 id를 의미하므로, 목적지 태그에 #(=id)을 중복 사용하지 않도록 주의한다.
## 파비콘 적용 순서
* `파비콘(favicon)`이란? - 웹을 구분 가능하게 하는 아이콘이다.
* 1. 파비콘 크기로 이미지 다운받거나 편집하기
* 2. html에서 head 안에 link 태그로 `favicon` href주소 연결하기
* 상황에 따라 달라지지 않고, 정해진 구조 그대로 코드를 복사+붙여넣기 해서 사용함.
* <link rel="shortcut icon" href="파비콘파일" type="image/x-icon">
* <link rel="icon" href="파비콘파일" type="image/x-icon">
## 이미지 태그 `img`
* `<img src="url(상대경로)" alt="">`
* inline 태그로, 블록 태그(h, p 등)와 형제일 수 없음. (형제로 쓰려면, p나 a와 같은 블록 태그에 감싸준다.)
* `대체텍스트  alt`는 정보를 전달하기 위한 내용을 작성한다.
* `대체텍스트  alt`는 이미지가 가진 의미 유무에 따라 이해하기 쉽게 작성한다.(ex : 텍스트 없는 이미지=의미x / 버튼=의미o)
* `<a href="#"><img src="상대경로"></a>` : img를 클릭했을때 지정한 경로(지정 페이지)로 이동한다.
## 이미지 태그 `img` (inline)
* 인라인 태그(em,strong, figcaption 등)과 형제 태그로 작성될 수 있다.
## figure, figcaption 태그
* `figure`는 블록, `figcaption`은 인라인 태그다.
* figure = 문서 안 사진 감싸는 틀 / figcaption = 사진 캡션
## video 태그 (block)
* 가능하면 모든 브라우저에 호환이 되는 .mp4 확장자를 쓰는 게 좋다.
* 1) 영상의 주소를 가져오는 방법(소스코드)은 주소 뒤에 `?autoplay=1&mute=1&loop=1` 등의 값을 입력해준다.
* 2) 내가 가진 영상(다운로드된 영상)은 열린 태그에 `<video src="비디오.mp4" autoplay muted loop controls>` 값을 작성한다.
## class, id 많이 사용하는 키워드
* wrapper, wrap, area 전체 묶는 영역
* contents, container 중~소 묶는 영역
* group, g 간단한 소그룹 영역
* top, btm, left, right 레이아웃 방향을 의미하는 키워드
* 예 : 의미있는단어_영역명
* 예시 : product_wrap, item_area, price_g, main_contents, top_btn
## div
* 인라인과 블록이 2개 이상 형제일 경우 묶어주는 그룹태그
* 레이아웃 기준 1행에 2열 이상 배치일 경우
* 특정 의미를 가진 행에 같은 디자인 요소가 배치된 경우
## span
* 인라인이 2개 이상 형제일 경우 묶는 그룹태그
* 의미없는 디자인 요소 인라인 처리 필요 시 사용
* span(인라인) 안에 img(인라인) 사용 가능
## semantic tag란?
* 레이아웃 태그
* header, section, footer 등이 있음
### header
* 사이트의 상단에서 '메뉴bar(gnb)'를 품고 있는 커다란 영역
### nav
* 내비게이션 태그
### gnb, lnb, snb
* gnb (global navigation bar) : nav 묶이는 대상 (사이트 제일 큰, 주요 메뉴)
* lnb (local navigation bar)
* snb (side navigation bar)
## ul, ol, li
* 목록 태그라고 하며, 크게 순차, 비순차 목록 태그가 있다.
* `ul`은 비순차 목록 태그 (li 이외에는 자식 태그 올 수 없다 / `ul`과 h,p 등등은 형제태그 가능)
* `ol`은 순차 목록 태그 (li 이외에는 자식 태그 올 수 없다 / `ol`과 h,p 등등은 형제태그 가능)
* `li`는 ul, ol과 항상 같이 써야 한다. (ul,ol: 부모 - li: 자식)
* `li`는 h,p,a 등등의 태그를 자식으로 둘 수 있다. (형제는 불가능)
* 따라서, `ul,ol태그` 과 `h,p,a 태그`는 `형제, 자손 관계`만 가능하다.
## details, summary
* `details` : 
* `summary` : 인라인 태그에 가깝다. (span(인라인)과 형제로 쓸 수 있음)
## footer, mark, main, time
* `footer` : 사이트의 하단에서 회사의 주소와 고객센터 정보 등등을 담고 있는 영역을 잡는 시멘틱 태그
* `mark` : 하이라이트 기능이 있는 인라인 태그
* `main` : header와 footer 사이 내용을 담는 커다란 영역을 잡는 시멘틱 태그
* `time` : 웹 사이트에서 시간을 기록해주는 태그