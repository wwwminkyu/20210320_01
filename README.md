### 문준석
- https://github.com/ministori-yonsei
- https://codepen.io/ministori-yonsei
### ministori@naver.com
>> 깃허브는 svn의 종류 중 하나다
>> TortoiseSVN 개인적으로 버전관리할 때 썼는데(설치) 요즘에는 깃허브를 쓴다
>> 깃 : 버전 컨트롤 시스템 중 하나다
>> OS : 리눅스(선마이크로 시스템즈의 유닉스를 카피) > 맥(리눅스 기반으로만듬) > 윈도우
>> 프론트엔드, 백엔드 로드맵

# 프론트 엔드 기초 수업

## GITHUB 기초 개념

> GITHUB 용어

- repository : 저장소, 프로젝트가 거주할 수 있는 디렉토리나 저장 공간. repo라고도 줄여 사용한다.
- stage : commit 할 대상을 선택
- commit : 수정한 내용의 스냅샷을 찍는다 (해당 시점의 스냅샷을 찍어 프로젝트를 재평가하거나 복원할 수 있는 체크포인트를 가질 수 있다. 깃허브에 저장)
- push : GITHUB 서버에 업로드
- stage -> commit -> push(네트워크에서 저장한거를 깃허브에 업로드하는것)
- pull : GITHUB 서버에서 다운로드
- branch : 각각의 개발자가 독립적으로 개발하기 위한 가지, master branch에 모두 접근해서 사용 시 오류 발생할 수 있음. 주 개발자 외 나머지는 다른 branch에서 개발 후 합치는 과정을 거침
- pull request : 각각의 branch에서 개발한 것을 master branch로 병합하기 위한 '요청'
- merge : 각각의 branch에서 개발한 것을 master branch로 병합하는 것
- 마크다운 문서 : 깃허브에 사용하는 문서파일 (.md)
- 컴퓨터 용어 중 WYSIWYG 위지위그 (마크다운 문서는 위지위그 방식이 아니다.)
- (What You See IS What You Get, 보는대로 얻는다), 편집화면과 출력화면이 같은 것 (예전에는 안그랬다고함), 대표 프로그램 : 워드, 한글 등 편집 툴
-
- 깃허브 작업 편하게하는 프로그램 - 소스트리 (계정생성 후 사용해보자)

> 사이트링크

마크다운 사용법 : [안내문서](https://gist.github.com/ihoneymon/652be052a0727ad59601)<br/>
HTLM, CSS, JS 참고 사이트 : [W3Schools](https://www.w3schools.com/)<br/>
온라인 에디터 : [Codepen](https://codepen.io/trending)<br/>
HTML 표 만들기 : [table generator](https://www.tablesgenerator.com/html_tables#)<br/>
심심할때 보는 노트북 정보 블로그 : [테크인포](https://blog.naver.com/techinfo112/222097528617)<br/>
2 : [노트북정보](https://blog.naver.com/hchanu48/222320866929)</br>
무료사진 : [저작권없는 무료사진 사이트 5개추천](https://m.blog.naver.com/kusshand_official/221032238202)<br/>
더미텍스트 영문 : [Lorem Ipsum](https://www.lipsum.com/)<br/>
더미텍스트 한글 : [한글입숨](http://hangul.thefron.me/)<br/>
한글자음키 : [특수문자표](http://kor.pe.kr/util/4/Special_char.htm)<br/>
프론트엔드 자료 : [MDN](https://developer.mozilla.org/ko/)<br/>
날씨API : [OpenWeather](https://openweathermap.org/)<br/>
개발자도구 : [제트브레인](https://www.jetbrains.com/ko-kr/)<br/>
[json parser](http://json.parser.online.fr/)
[카카오지도](https://apis.map.kakao.com/)<br/>
[카카오개발자](https://developers.kakao.com/)</br>
호스팅:[닷홈](http://wwwminkyu.dothome.co.kr/html/)</br>
FTP:[Filezilla](https://filezilla-project.org/download.php?type=client#close)

## WEB/IT 기초 개념

> 클라이언트 서버 모델

<img src="https://github.com/wwwminkyu/20210320_01/blob/main/1200px-Client-server-model.svg.png" width="648" />

클라이언트-서버 모델에서 클라이언트는 사용자가 사용하는 디바이스(PC, Mobile)를 의미하고, 서버는 클라이언트가 접속해서 데이터나 파일을 요청했을때 응답하는 시스템.

클라이언트와 서버는 네트워크를 통해서 연결됨

<img src="https://s3-ap-northeast-2.amazonaws.com/opentutorials-user-file/course/2614/4971.png" />

클라이언트와 서버 모델은 실제 연결은 아니지만 개념적으 클라이언트 관점에서 1:1로 연결되었다고 생각할 수 있음

클라이언트-서버 모델에서 이루어지는 동작은 클라이언트의 요청(request)과 서버의 응답(response)의 1 사이클로 구성됨

클라이언트는 클라이언트 디바이스에서 실행되는 웹브라우저, 서버는 서버 디바이스에서 실행되는 서버 소프트웨어가 실제로 사용되는 것임

## HTML

> [HTML Introduction](https://www.w3schools.com/html/html_intro.asp)<br/>
- 하이퍼텍스트 표시 언어, 웹 페이지 구조 설명, 해당 콘텐츠가 어떤 콘텐츠(제목/단락/링크)인지 표시해주는 언어
- 중요 !! 어떤 태그를 달까 생각하지말고, 어떤 콘텐츠인지를 우선 생각하는 사고를 갖자
- 전체 HTML 영역에 head tag영역(사이트를 설명하는 정보, 탭 제목 등)과 body tag영역(웹 페이지 내 콘텐츠)이 나눠져있다. 
> [HTML Elements](https://www.w3schools.com/html/html_elements.asp)<br/>
- < tagname > 여기에 콘텐츠 입력 ... < / tagname >
- 일부 HTML 요소의 예 : <br>
< h1 > 나의 첫 번째 제목 < / h1 ><br>
< p > 내 첫 단락. < / p ><br>
> [HTML Attributes](https://www.w3schools.com/html/html_attributes.asp)<br/>
- HTML 속성 (CSS의 속성 단어 - property +와 다르다)
1) HTML Element에 추가 정보를 제공
2) name = "value" 형태로 사용
- src 속성 : 화상의 경로를 표시하는 속성 지정- src 속성 : 화상의 경로를 표시하는 속성 지정<br/>

> 웹 문서에서 표시할 수 있는 콘텐츠
1) 텍스트
2) 이미지
3) 멀티미디어(비디오, 오디오)

### 텍스트 콘텐츠 요소(

> [HTML Headings](https://www.w3schools.com/html/html_headings.asp)<br/>
- 제목 태그
- Heading -> h
- h1 ~ h6
> [HTML Paragraphs](https://www.w3schools.com/html/html_paragraphs.asp)<br/>
- 단락 태그
- Paragraph -> p
- 수평선
- Horizontal Rules -> hr (Empty Element)
> [HTML Links](https://www.w3schools.com/html/html_links.asp)<br/>
- 하이퍼링크
- Anchor -> a
href : 링크로 연결된 목적지 주소
1) 외부링크
- 링크 주소 입력 시 http(https) 키워드를 사용
3) 북마크
- 목적지에 id attribute를 사용해서 이름을 정해줌
- href attribute에 #를 사용해서 목적지 이름을 입력

> [HTML Tables](https://www.w3schools.com/html/html_tables.asp)<br/>
- [table generator](https://www.tablesgenerator.com/html_tables#)<br/>

> [HTML Lists](https://www.w3schools.com/html/html_lists.asp)<br/>
1) 순서없는 목록 (ul)
2) 순서있는 목록 (ol)
3) 설명 목록
- ul, ol 목록에서 중첩(nested) 형태로 사용할때 포함 관계를 주의
- 포함하는 목록 항목에 작은 목록 전체가 포함됨


### 이미지 콘텐츠 요소
> [HTML Images](https://www.w3schools.com/html/html_images.asp)</br>
1) src attribute : 가져올 이미지 파일 위치 정보
2) alt(alternative) attribute : 대체 텍스트

### 멀티미디어 콘텐츠 요소
> [HTML Video](https://www.w3schools.com/html/html5_video.asp)
- attribute의 형태
1) name = "value"
2) name만 사용
- video 태그의 attribute
1) controls
2) autoplay
3) muted
4) loop

> [HTML YouTube Videos](https://www.w3schools.com/html/html_youtube.asp)
- youtube의 매개변수
1) controls -> youyube_url/VIDEO_ID?controls=1
2) autoplay -> youyube_url/VIDEO_ID?autoplay=1
3) mute -> youyube_url/VIDEO_ID?mute=1
4) loop -> youyube_url/VIDEO_ID?loop=1&playlist=VIDEO_ID
- 여러 매개변수 동시 사용
- youtube_url/VIDEO_ID?controls=1&autoplay=1&mute=1&loop=1&playlist=VIDEO_ID (& : ampersand) <-루프는 플레이리스트를 추가해야 적용된다.


### HTML5 Content Model
> Sectioning Contents
- Semantic Element

> [HTML Semantic Elements](https://www.w3schools.com/html/html5_semantic_elements.asp)
1) 특정 의미를 부여해준 Containor 요소
2) 레이아웃 구성할 때 각각의 영역을 구분하기 위해 사용

참고링크
- [Photopea](https://www.photopea.com/)
- [Website Template](https://freebiesbug.com/psd-freebies/piroll-design-template-agencypersonal-portfolio/)
- 수업때 사용한 파일, 여기에 내용 추가하여 나머지도 영역 나눠오기 숙제[01_One Page.zip](https://github.com/wwwminkyu/20210320_01/files/6252184/01_One.Page.zip)

### 프론트엔드 기술 (HTML, CSS, JS)의 브라우저 지원 여부 체크
- 프론트엔드 기술이 버전업 될때마다 브라우저가 지원하는지 체크할 필요가 있음.
- HTML5/5.1 , CSS3 , ES2015이후 버전들의 기술은 항상 지원여부 체크가 필요함.
- 브라우저 지원여부
- 상위 호환성 : 새 버전 브라우저의 지원 여부
- 하휘 호환성 : 구 버전 브라우저의 지원 여부
- 일반적으로 브라우저 지원은 하위 호환성 체크가 중요함
- [Can I Use](https://caniuse.com/)

[HTML Block and Inline Elements](https://www.w3schools.com/html/html_blocks.asp)
- Non-sementic element
  - div(division)
  - span

### Blaoc/Inline Element
- block : 새 줄(줄바꿈)에서 표시
- inline : 한 줄에 나란히 표시
- 포함관계
  - block : block, inline, contents(text) 모두 포함할 수 있음
  - inline : inline, contents(text) 만 포함 가능
  - 예외 : inline요소인 a 태그는 모두 포함 가능

### 폼 요소
- 사용자 입력을 받을 수 있는 요소
> [HTMLForm Elements](https://www.w3schools.com/html/html_form_elements.asp)

> 텍스트 입력 폼 요소
```
<input type="text" /> : 한 줄 입력
<textarea></textarea> : 여러 줄 입력
<input type="password" /> : 한 줄 입력, 입력 내용이 기호로 표시
```
> 파일 업로드 폼 요소
```
<input type="file" />
```
> 선택 폼 요소
```
<input type="radio" />
<input type="checkbox" />
<select>
    <option></option> : 목록 항목
  </select>
```  
> 실행 폼 요소
```
<input type="button" />
<input type="reset" />
<input type="submit" />
<button type="button" /></button>
<button type="reset" /></button>
- <button type="submit" /></button>
```

### HTML Element에 이름 붙이기 (-> CSS에서 사용하려고)

> id와 class를 사용한다. (html요소에 하나하나씩 이름을 붙힌다. 모두 attribute 형태로!)
 ```
<p id ="paragraph1">단락</p>
<p class="paragraph2"></p>
```
> id와 class의 차이 
> (프론트엔드에서는 class만 쓰자! 백엔드에서 id사용할 가능성이 많아서 중복 방지!)
- id는 하나의 HTML 파일(문서)에서 중복 사용될 수 없음
- class는 하나의 HTML 파일(문서)에서 중복 사용할 수 있음(CSS styling, Javascript 기능을 동시 적용)

> 표기법(여러단어가 사용될경우 단어를 구분)
- gna-list-item : kebab case
- gnb_list_item : snake case
- gnbListItem : camel case
- GnbListItem : Pascal case

- 파일, 폴더 이름 : snake case
- id, class : kebab case
- 자바스크립트 변수, 함수 : camel case

### 박스 가로 배치

> float 
- left, right 속성값으로 가로배치
- 부모 요소를 기준으로 왼쪽배치, 오른쪽 배치
- right 값을 사용하면 박스 순서가 반대로 배치
- 박스는 가로는 부모요소 길이, 세로는 자식요소 길이다 (인라인 단독으로 가로 세로 정해주면 적용안됨)
- 레이아웃을 올바르게 하기위해 부모요소의 높이를 높인다 또는 float으로 적용한 박스의 위치를 정한다 (미리 한번 더 묶는거)

> [리셋 CSS ](https://meyerweb.com/eric/tools/css/reset/)
> [구글웹폰트](https://fonts.google.com/?subset=korean)

### 반응형 웹(Responsive Web)

> OSMU(One Source Multi Use) - One Sourse => HTML
> 적응형 웹(Adaptive Web) - OSMU가 적용되지 않음
> 


### JavaScript

- 객체 oocss처럼 어떤 것이든 객체화 한다.
- 프로그래밍언어의 객체는 크게 properties와 methods를 갖고있다.
- JSP프로그래밍을 한다고 하면 이미 만들어놓은 객체를 활용한다. 이미 가져와서 적절하게 조합. 그러면 어떤 객체를 쓸것인가.
- 객체가 갖고있는 properties와 methods를 어떻게 쓸 것인가.
- properties : 겉으로 나타나는 표현해주는, 속성
- methods : 동작과 관련된 괄호가 있다.
- JSP는 HTML을 목적으로한다.
- HTML을 객체화 하는 것을 DOM(Document Object Model)이라고 한다.
- 



- 
