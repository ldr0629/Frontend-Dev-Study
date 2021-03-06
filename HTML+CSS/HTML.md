# HTML Basic and Syntax

## HTML 
웹의 최소 단위인 웹 페이지를 만드는 언어이고, HTML을 구성하고 있는 최소의 단위는 태그(tag)이다.

언어라는 관점에서 보았을 때 웹 브라우저라고 하는 프로그램과 사람 사이에서 서로가 이해할 수 있는 약속이라고 할 수 있다.

태그를 사용할 때 항상 시작태그 ~ 닫히는 태그(/태그명)으로 사용된다. <br>
공백 및 줄바꿈은 웹페이지에서 무시하기 때문에 태그를 사용해주어야 한다.

**head, body** <br>
본질적인 정보와 부가적인 정보로 나뉘어 각각 다른 태그에 담도록 "약속"이 되어있는데 이 때 사용하는 태그이며 본문이 아닌 태그는 <'head'> 태그 안에 들어오고, 본문인 태그는 <'body'> 태그 안에 들어온다.

웹 페이지의 기본적인 구조를 짜는데 필요한 태그이며, <'head'> 태그 작성 후 원하는 제목을 탭에 보이게 하고싶을 때 <'title'> 태그를, 문서의 부가적인 정보나 형식을 맞추고자 할 때 <'meta'> 태그를 사용한다.

**h1 ~ h6** <br>
- 제목은 굵고 큰 문자로 꾸며주고 줄바꿈을 한다는 태그로, 소제목을 쓰고 싶은경우 h 뒤에 숫자를 줄여가며 사용한다.

**strong** <br>
- 뒤에 나오는 문자들을 진하게 표시 하는 태그

**a** <br>
- <'a'> 태그 안쪽에 있는 부분이 링크라는 사실을 브라우저에게 알려주는 태그이며
어떤 웹 페이지와 연결되어 있는가에 관한 URL을 명시해줘야 한다. 태그명만으로는 정보가 불충분하므로 URL을 명시해주는 것인데 이때 "href"라는  속성의 이름 값을 이용한다. 이 앵커 태그는 HTML 문서의 특정위치로 이동하기 위함이다.

- 새로운 탭이 열리면서 거기에서 페이지가 열리게 하고 싶을 때 "target"이라는 속성의 "_blank" 값을 사용한다. "target"은 링크에 연결된 웹 페이지가 출력될 탭을 지정할 때 쓴다.

**li** <br>
- 목록으로 웹페이지를 표현하고 싶을 때, 각각의 항목들을 리스트로 표현하는 <''li'> 태그를 이용하며 시각적으로 구별할 수 있다. 

- 단독적으로 사용하진 않으며 순서가 없는 리스트로 표현할 땐 <'ul'>(unordered list) 태그를, 순서가 있는 리스트일 때는 <'ol'>(ordered list) 태그를 사용한다.

- 어떠한 용어에 대해 정의를 내릴 때 사용하는 <'dl'>(definition list)도 있으며 각 단어마다 <'dt'>와 <'dd'> 태그로 감싸준다.

**p** <br>
- 단락을 표현할 때 사용하는 태그이고 줄바꿈의 간격은 고정되어 있다.

**br** <br>
- 자유롭게 간격을 조정하고 싶은 경우의 줄바꿈 태그이며, void element로서 내용이 없는 태그이다. 또한, 닫히는 태그가 없다.

**img** <br>
- 웹 페이지에 이미지를 포함할 수 있는 태그이다. 이 태그 또한 닫히는 태그가 없어도 사용할 수 있으며 "src" 속성을 이용하여 파일, 확장자명을 작성해주어야 한다.

- 이미지가 깨졌을 때를 방지해 텍스트를 작성할 수 있는 "alt" 속성, 너비와 높이를 지정해줄 수 있는 "width", "height" 속성 등이 있다.

**table** <br>
- 웹 페이지에 표를 삽입하고자 할 때 쓸 수 있고, 테이블을 표현하는데 항목 하나하나는 <'td'>(table data) 태그로 묶어준다.

- <'td'>로 묶어준 태그들은 하나의 행으로 그룹핑 시켜주기 위해 <'tr'>(table row) 태그를 사용한다. 테두리를 지정할 때에는 "border" 속성으로 styling 해준다.

- 웹 페이지에 담겨있는 정보를 더 가치있게 만드려면 이들을 구조화할 필요가 있는데, <'thead'>, <'tbody'>, <'tfoot'> 태그를 사용할 수 있다.

- 테이블을 구성하고 일부분 표를 병합하는 방법으로 "rowspan", "colspan" 속성을 활용한다.

**form** <br>
- 사용자가 입력한 정보를 서버로 전송할 때 이용하는 태그이며, 입력 양식을 제공하는 태그로 <'input'>이 있다.

- 단순 텍스트를 입력해야 하는 경우 "type"의 속성 값으로 text를, 비밀번호 형태로 표현하는 경우 password를, 서버로 전송하는 버튼을 나타낼 때는 submit, 사용자 입력을 초기화하는 reset이 있으며 이외의 다양한 형식을 제공하고 있다.

- 입력한 정보에 대해 어떤 서버로 전송이 될 것인지 명시해주지 않아 "action" 속성을 이용해 이 속성값으로 submit 버튼을 눌렀을 때 브라우저는 지정된 웹 서버 응용 프로그램 실행을 요청할 수 있다.

- 입력한 정보에 대해 경우에 따라 URL로 전달하는 게 필요할 때(get)가 있고 보안적으로 숨기고자 할 때(post)가 있는데 "method" 속성으로 이를 지정해준다. default value는 get이며, 서버로 데이터를 전송한다면 대부분 post 방식을 이용한다.

- <'textarea'> : 텍스트 입력 박스에 입력할 때 여러 줄을 입력받을 때 사용.
- <'option'> : 각각의 항목을 선택지로 정의를 하기위해 사용하는 태그로, <'select'> 태그로 감싸주어야 한다.
- radio, checkbox : input 태그의 type이며 여러 개의 선택지 중 하나 또는 복수 개를 선택해서 제출할 수 있도록 하는 방법이며 UI로 사용된다. 기본적으로 어떠한 항목을 선택되게 하고 싶다면 "checked" 속성을 활용한다.

**iframe** <br>
- 웹 페이지에 다른 웹 문서를 삽입하는 방법으로, "src" 속성을 이용해서 어떤 웹 페이지를 삽입할 것인지 지정해주어야 한다. 

- 보안상 신뢰할 수 없는 사이트에서 악성코드 같은 취약 요소를 포함하고 있다면 외부소스로부터 실행될 수 있기때문에 이를 방지하려면 "sandbox" 속성을 작성해줄 필요도 있다.

**video and audio** <br>
- 비디오와, 오디오를 웹 문서 내 삽입하기 위한 태그로 <'source'> 태그를 이용하거나 "src" 속성을 이용해서 링크를 걸어줄 수 있다.

- 비디오의 크기는 "width", "height"로 지정하며 이외에도 컨트롤러를 제공하는 "controls", 자동 재생이 가능한 "autoplay" 등이 있다.

## Semantic tags
여러 가지 정보들을 의미에 맞게 잘 표현하기 위한 태그들이 있으며 어떻게하면 정보로서 가치를 높일 수 있는가에 관한 내용이다.

**header** <br>
- 웹 페이지 section의 머리말 표현, 페이지 제목, 페이지를 소개할 때 일반적으로 상단에 쓰이는 태그이다.

**nav** <br>
- 하이퍼링크들을 모아 놓은 특별한 섹션, 페이지 내 목차를 만드는 용도

**section** <br>
- 문서의 챕터 혹은 절을 구성하는 역할로 여러 섹션으로 구성할 수 있다.

**article** <br>
- 특정 부분이 본문이라는 것을 의미론적으로 표현할 수 있고, <'section'> 태그로 묶어주는 경우도 많다.

**aside** <br>
- 본문에서 벗어난 내용을 표시하고자 할 때, 페이지의 오른쪽 또는 왼쪽에 주로 배치된다.

**footer** <br>
- 웹 페이지 하단에 어떤 정보를 표현할 때 작성되며 꼬리말 영역에 해당된다. 예를 들면 저자나 저작권 정보가 이 태그 내에 컨텐츠로 사용될 수 있다.
