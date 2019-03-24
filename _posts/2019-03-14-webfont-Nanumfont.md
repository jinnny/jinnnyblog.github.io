---
title: "[CSS] 나눔시리즈 경량화 웹폰트와 CDN"
date: 2019-03-14 16:00:00 -0400
categories: CSS 폰트경량화 웹폰트 CDN 
tags: CSS 나눔바른고딕 나눔스퀘어 나눔스퀘어라운드 
---

나눔시리즈 폰트로 웹폰트 경량화 진행하기
=======


작업에 앞서..
---

웹폰트와 최적화에 대한 포스팅을 했었지만, 
웹폰트에 대한 고민은 늘 하고 있기에 나눔시리즈를 대상으로 웹폰트와 CDN을 진행하고자 포스팅을 하게 되었습니다.  
폰트를 웹에 적용하는 것은 참 쉽지 않은 작업 같습니다. 한글은 한자와 함께 폰트가 만들어지는 경우가 많기때문에 자동적으로 부피가 커지기 때문입니다.  

그러나 자주사용하는 한글에 대한 웹폰트를 서브셋으로 만들게 되면 한자를 사용할 경우나 커뮤니티와 같이 사용자가 어떤 글자를 쓸지 모를 상황에서 난감한 것 같습니다. 
현재 존재하는 커뮤니티 성격을 띄는 사이트를 살펴보니 굴림체, 돋움체와 같은 기본 폰트를 쓰는 것을 쉽게 찾아 볼 수 있었습니다.  
사용자가 글을 쓰는 게시판 부분에는 기본 폰트를 사용하고, 그 외 부분에는 기본 폰트가 아닌 다른 폰트를 사용하는 것도 하나의 방법이라 생각도 들었는데,
그런 경우에는 이질감이 생길 우려도 있는 것 같습니다.

그래서 기본적으론 서브셋을 만들되, 사이트의 목적에 따라 서브셋을 사용하지 않는 쪽이 좋을 것 같습니다.  

이번에 웹폰트로 만들어 CDN 으로 공유할 나눔시리즈는 아래와 같습니다.

1. '나눔바른고딕'
2. '나눔스퀘어'
3. '나눔스퀘어라운드'
4. '나눔바른펜'
5. '나눔손글씨붓/펜'
6. '나눔고딕'
7. '나눔명조'

서브셋 작업은 용량이 큰 '나눔바른고딕', '나눔바른펜', '나눔손글씨붓/펜', '나눔고딕', '나눔명조'를 진행했습니다.


---

1. 나눔바른고딕 (NanumBarunGothic)
----
나눔바른고딕은 한글 11,172자, 한자 4,888자, 영문 94자, KS약물 986자 로 구성되어있으며,
ttf 기준 용량은 4.2MB ~ 4.9MB 입니다.
서브셋 경량화 작업을 통해 용량은 1.3MB ~ 1.8MB 로 줄었습니다.

**1. 지원 언어 (경량화 후 기준)**    
 1. 영어
 2. 한국어 (한자 불포함)
  
**2. 종류**  
1. UltraLight
2. Light
3. Regular 
4. Bold

**4. CDN 사용법**  

```
@import url('https://jinnny.github.io/publish_source/webfont/NanumBarunGothic/fonts.css');
```

```
font-family: 'NanumBarunGothic', Dotum ,'돋움', sans-serif;
```


2. 나눔스퀘어 (NanumSquare)
----
나눔스퀘어는 한글 2,350자, 영문 94자, KS약물 986자로 구성되어있으며,
ttf 기준 용량은 724KB ~ 751KB 입니다.

**1. 지원 언어**    
 1. 영어
 2. 한국어 (한자 불포함)
  
**2. 종류**  
1. Light
2. Regular 
3. Bold
4. ExtraBold

**3. CDN 사용법**  

```
@import url('https://jinnny.github.io/publish_source/webfont/NanumSquare/fonts.css');
```

```
font-family: 'NanumSquare', Dotum ,'돋움', sans-serif;
```


3. 나눔스퀘어라운드 (NanumSquareRound)
----
나눔스퀘어라운드는 한글 2,350자, 영문 94자, KS약물 986자로 구성되어있으며,
ttf 기준 용량은 1MB ~ 1.1MB 입니다.

**1. 지원 언어**    
 1. 영어
 2. 한국어 (한자 불포함)
  
**2. 종류**  
1. Light
2. Regular 
3. Bold
4. ExtraBold

**3. CDN 사용법**  

```
@import url('https://jinnny.github.io/publish_source/webfont/NanumSquareRound/fonts.css');
```

```
font-family: 'NanumSquareRound', Dotum ,'돋움', sans-serif;
```

4. 나눔바른펜 (NanumBarunPen)
----
나눔바른펜은 한글 11,172자, 영문 94자, KS약물 986자로 구성되어있으며,
ttf 기준 용량은 10MB ~ 11MB 입니다.
서브셋 경량화 작업을 통해 용량은 1.9MB ~ 2.0MB 로 줄었습니다.


**1. 지원 언어 (경량화 후 기준)**    
 1. 영어
 2. 한국어 (한자 불포함)
  
**2. 종류**  
1. Regular 
2. Bold

**3. CDN 사용법**  

```
@import url('https://jinnny.github.io/publish_source/webfont/NanumBarunPen/fonts.css');
```

```
font-family: 'NanumBarunPen', Dotum ,'돋움', sans-serif;
```

5. 나눔손글씨붓/나눔손글펜 (NanumBrush/NanumPen)
----
나눔손글씨붓/펜은 한글 2,350자, 영어 94자, KS약물 986자로 구성되어있으며,
ttf 기준 용량은 3.5MB ~ 3.7MB 입니다.
서브셋 경량화 작업을 통해 용량은 1.9MB ~ 2.1MB 로 줄었습니다.


**1. 지원 언어 (경량화 후 기준)**    
 1. 영어
 2. 한국어 (한자 불포함)
  
**2. 종류**  
1. Regular 


**3. CDN 사용법**  

```
@import url('https://jinnny.github.io/publish_source/webfont/NanumBrushPen/fonts.css');
```

```
//나눔손글씨붓
font-family: 'NanumBrush', Dotum ,'돋움', sans-serif;

//나눔손글씨펜
font-family: 'NanumPen', Dotum ,'돋움', sans-serif;
```

6. 나눔고딕 (NanumGothic)
----
나눔고딕은 Light, Regular, Bold, Extra Bold의 경우, 한글 11,172자, 한자 4,888자, 영문 94자, KS약물 986자로 구성되어 있고,
Light의 경우에는 한글 2,350자, 영문 94자, KS약물 986자로 구성되어있으며, ttf 기준 용량은 1.5MB ~ 4.7MB 입니다.
서브셋 경량화 작업을 통해 용량은 1.4MB ~ 1.6MB 로 줄었습니다.

**1. 지원 언어 (경량화 후 기준)**    
 1. 영어
 2. 한국어 (한자 포함)
  
**2. 종류**  
1. Light
2. Regular 
3. Bold
4. ExtraBold

**3. CDN 사용법**  

```
@import url('https://jinnny.github.io/publish_source/webfont/NanumGothic/fonts.css');
```

```
font-family: 'NanumGothic', Dotum ,'돋움', sans-serif;
```

7. 나눔명조 (NanumMyeongjo)
----
나눔명조는 한글 11,172자, 영문 94자, KS약물 986자로 구성되어있으며,
ttf 기준 용량은 3.8MB ~ 4.8MB 입니다.
서브셋 경량화 작업을 통해 용량은 2.4MB ~ 3.2MB 로 줄었습니다.


**1. 지원 언어 (경량화 후 기준)**    
 1. 영어
 2. 한국어 (한자 불포함)
  
**2. 종류**  
1. Regular 
2. Bold
3. ExtraBold

**3. CDN 사용법**  

```
@import url('https://jinnny.github.io/publish_source/webfont/NanumMyeongjo/fonts.css');
```

```
font-family: 'NanumMyeongjo', Dotum ,'돋움', sans-serif;
```
  

**서브셋 지정 글자**  
---
  
```
KS X 1001 완성형 한글 2,340자
        +   
노민지, 윤민구 “KS 코드 완성형 한글의 추가 글자 제안” 추가 글자 224자
        +
현대 한글의 낱자 51자
        +
Basic Latin 95자
       +
KS X 1001의 특수 문자 942자
```
로 아래와 같습니다.
```
가각간갇갈갉갊감갑값갓갔강갖갗같갚갛개객갠갤갬갭갯갰갱갸갹갼걀걋걍걔걘걜거걱건걷걸걺검겁것겄겅겆겉겊겋게겐겔겜겝겟겠겡겨격겪견겯결겸겹겻겼경곁계곈곌곕곗고곡곤곧골곪곬곯곰곱곳공곶과곽관괄괆괌괍괏광괘괜괠괩괬괭괴괵괸괼굄굅굇굉교굔굘굡굣구국군굳굴굵굶굻굼굽굿궁궂궈궉권궐궜궝궤궷귀귁귄귈귐귑귓규균귤그극근귿글긁금급긋긍긔기긱긴긷길긺김깁깃깅깆깊까깍깎깐깔깖깜깝깟깠깡깥깨깩깬깰깸깹깻깼깽꺄꺅꺌꺼꺽꺾껀껄껌껍껏껐껑께껙껜껨껫껭껴껸껼꼇꼈꼍꼐꼬꼭꼰꼲꼴꼼꼽꼿꽁꽂꽃꽈꽉꽐꽜꽝꽤꽥꽹꾀꾄꾈꾐꾑꾕꾜꾸꾹꾼꿀꿇꿈꿉꿋꿍꿎꿔꿜꿨꿩꿰꿱꿴꿸뀀뀁뀄뀌뀐뀔뀜뀝뀨끄끅끈끊끌끎끓끔끕끗끙끝끼끽낀낄낌낍낏낑나낙낚난낟날낡낢남납낫났낭낮낯낱낳내낵낸낼냄냅냇냈냉냐냑냔냘냠냥너넉넋넌널넒넓넘넙넛넜넝넣네넥넨넬넴넵넷넸넹녀녁년녈념녑녔녕녘녜녠노녹논놀놂놈놉놋농높놓놔놘놜놨뇌뇐뇔뇜뇝뇟뇨뇩뇬뇰뇹뇻뇽누눅눈눋눌눔눕눗눙눠눴눼뉘뉜뉠뉨뉩뉴뉵뉼늄늅늉느늑는늘늙늚늠늡늣능늦늪늬늰늴니닉닌닐닒님닙닛닝닢다닥닦단닫달닭닮닯닳담답닷닸당닺닻닿대댁댄댈댐댑댓댔댕댜더덕덖던덛덜덞덟덤덥덧덩덫덮데덱덴델뎀뎁뎃뎄뎅뎌뎐뎔뎠뎡뎨뎬도독돈돋돌돎돐돔돕돗동돛돝돠돤돨돼됐되된될됨됩됫됴두둑둔둘둠둡둣둥둬뒀뒈뒝뒤뒨뒬뒵뒷뒹듀듄듈듐듕드득든듣들듦듬듭듯등듸디딕딘딛딜딤딥딧딨딩딪따딱딴딸땀땁땃땄땅땋때땍땐땔땜땝땟땠땡떠떡떤떨떪떫떰떱떳떴떵떻떼떽뗀뗄뗌뗍뗏뗐뗑뗘뗬또똑똔똘똥똬똴뙈뙤뙨뚜뚝뚠뚤뚫뚬뚱뛔뛰뛴뛸뜀뜁뜅뜨뜩뜬뜯뜰뜸뜹뜻띄띈띌띔띕띠띤띨띰띱띳띵라락란랄람랍랏랐랑랒랖랗래랙랜랠램랩랫랬랭랴략랸럇량러럭런럴럼럽럿렀렁렇레렉렌렐렘렙렛렝려력련렬렴렵렷렸령례롄롑롓로록론롤롬롭롯롱롸롼뢍뢨뢰뢴뢸룀룁룃룅료룐룔룝룟룡루룩룬룰룸룹룻룽뤄뤘뤠뤼뤽륀륄륌륏륑류륙륜률륨륩륫륭르륵른를름릅릇릉릊릍릎리릭린릴림립릿링마막만많맏말맑맒맘맙맛망맞맡맣매맥맨맬맴맵맷맸맹맺먀먁먈먕머먹먼멀멂멈멉멋멍멎멓메멕멘멜멤멥멧멨멩며멱면멸몃몄명몇몌모목몫몬몰몲몸몹못몽뫄뫈뫘뫙뫼묀묄묍묏묑묘묜묠묩묫무묵묶문묻물묽묾뭄뭅뭇뭉뭍뭏뭐뭔뭘뭡뭣뭬뮈뮌뮐뮤뮨뮬뮴뮷므믄믈믐믓미믹민믿밀밂밈밉밋밌밍및밑바박밖밗반받발밝밞밟밤밥밧방밭배백밴밸뱀뱁뱃뱄뱅뱉뱌뱍뱐뱝버벅번벋벌벎범법벗벙벚베벡벤벧벨벰벱벳벴벵벼벽변별볍볏볐병볕볘볜보복볶본볼봄봅봇봉봐봔봤봬뵀뵈뵉뵌뵐뵘뵙뵤뵨부북분붇불붉붊붐붑붓붕붙붚붜붤붰붸뷔뷕뷘뷜뷩뷰뷴뷸븀븃븅브븍븐블븜븝븟비빅빈빌빎빔빕빗빙빚빛빠빡빤빨빪빰빱빳빴빵빻빼빽뺀뺄뺌뺍뺏뺐뺑뺘뺙뺨뻐뻑뻔뻗뻘뻠뻣뻤뻥뻬뼁뼈뼉뼘뼙뼛뼜뼝뽀뽁뽄뽈뽐뽑뽕뾔뾰뿅뿌뿍뿐뿔뿜뿟뿡쀼쁑쁘쁜쁠쁨쁩삐삑삔삘삠삡삣삥사삭삯산삳살삵삶삼삽삿샀상샅새색샌샐샘샙샛샜생샤샥샨샬샴샵샷샹섀섄섈섐섕서석섞섟선섣설섦섧섬섭섯섰성섶세섹센셀셈셉셋셌셍셔셕션셜셤셥셧셨셩셰셴셸솅소속솎손솔솖솜솝솟송솥솨솩솬솰솽쇄쇈쇌쇔쇗쇘쇠쇤쇨쇰쇱쇳쇼쇽숀숄숌숍숏숑수숙순숟술숨숩숫숭숯숱숲숴쉈쉐쉑쉔쉘쉠쉥쉬쉭쉰쉴쉼쉽쉿슁슈슉슐슘슛슝스슥슨슬슭슴습슷승시식신싣실싫심십싯싱싶싸싹싻싼쌀쌈쌉쌌쌍쌓쌔쌕쌘쌜쌤쌥쌨쌩썅써썩썬썰썲썸썹썼썽쎄쎈쎌쏀쏘쏙쏜쏟쏠쏢쏨쏩쏭쏴쏵쏸쐈쐐쐤쐬쐰쐴쐼쐽쑈쑤쑥쑨쑬쑴쑵쑹쒀쒔쒜쒸쒼쓩쓰쓱쓴쓸쓺쓿씀씁씌씐씔씜씨씩씬씰씸씹씻씽아악안앉않알앍앎앓암압앗았앙앝앞애액앤앨앰앱앳앴앵야약얀얄얇얌얍얏양얕얗얘얜얠얩어억언얹얻얼얽얾엄업없엇었엉엊엌엎에엑엔엘엠엡엣엥여역엮연열엶엷염엽엾엿였영옅옆옇예옌옐옘옙옛옜오옥온올옭옮옰옳옴옵옷옹옻와왁완왈왐왑왓왔왕왜왝왠왬왯왱외왹왼욀욈욉욋욍요욕욘욜욤욥욧용우욱운울욹욺움웁웃웅워웍원월웜웝웠웡웨웩웬웰웸웹웽위윅윈윌윔윕윗윙유육윤율윰윱윳융윷으윽은을읊음읍읏응읒읓읔읕읖읗의읜읠읨읫이익인일읽읾잃임입잇있잉잊잎자작잔잖잗잘잚잠잡잣잤장잦재잭잰잴잼잽잿쟀쟁쟈쟉쟌쟎쟐쟘쟝쟤쟨쟬저적전절젊점접젓정젖제젝젠젤젬젭젯젱져젼졀졈졉졌졍졔조족존졸졺좀좁좃종좆좇좋좌좍좔좝좟좡좨좼좽죄죈죌죔죕죗죙죠죡죤죵주죽준줄줅줆줌줍줏중줘줬줴쥐쥑쥔쥘쥠쥡쥣쥬쥰쥴쥼즈즉즌즐즘즙즛증지직진짇질짊짐집짓징짖짙짚짜짝짠짢짤짧짬짭짯짰짱째짹짼쨀쨈쨉쨋쨌쨍쨔쨘쨩쩌쩍쩐쩔쩜쩝쩟쩠쩡쩨쩽쪄쪘쪼쪽쫀쫄쫌쫍쫏쫑쫓쫘쫙쫠쫬쫴쬈쬐쬔쬘쬠쬡쭁쭈쭉쭌쭐쭘쭙쭝쭤쭸쭹쮜쮸쯔쯤쯧쯩찌찍찐찔찜찝찡찢찧차착찬찮찰참찹찻찼창찾채책챈챌챔챕챗챘챙챠챤챦챨챰챵처척천철첨첩첫첬청체첵첸첼쳄쳅쳇쳉쳐쳔쳤쳬쳰촁초촉촌촐촘촙촛총촤촨촬촹최쵠쵤쵬쵭쵯쵱쵸춈추축춘출춤춥춧충춰췄췌췐취췬췰췸췹췻췽츄츈츌츔츙츠측츤츨츰츱츳층치칙친칟칠칡침칩칫칭카칵칸칼캄캅캇캉캐캑캔캘캠캡캣캤캥캬캭컁커컥컨컫컬컴컵컷컸컹케켁켄켈켐켑켓켕켜켠켤켬켭켯켰켱켸코콕콘콜콤콥콧콩콰콱콴콸쾀쾅쾌쾡쾨쾰쿄쿠쿡쿤쿨쿰쿱쿳쿵쿼퀀퀄퀑퀘퀭퀴퀵퀸퀼큄큅큇큉큐큔큘큠크큭큰클큼큽킁키킥킨킬킴킵킷킹타탁탄탈탉탐탑탓탔탕태택탠탤탬탭탯탰탱탸턍터턱턴털턺텀텁텃텄텅테텍텐텔템텝텟텡텨텬텼톄톈토톡톤톨톰톱톳통톺톼퇀퇘퇴퇸툇툉툐투툭툰툴툼툽툿퉁퉈퉜퉤튀튁튄튈튐튑튕튜튠튤튬튱트특튼튿틀틂틈틉틋틔틘틜틤틥티틱틴틸팀팁팃팅파팍팎판팔팖팜팝팟팠팡팥패팩팬팰팸팹팻팼팽퍄퍅퍼퍽펀펄펌펍펏펐펑페펙펜펠펨펩펫펭펴편펼폄폅폈평폐폘폡폣포폭폰폴폼폽폿퐁퐈퐝푀푄표푠푤푭푯푸푹푼푿풀풂품풉풋풍풔풩퓌퓐퓔퓜퓟퓨퓬퓰퓸퓻퓽프픈플픔픕픗피픽핀필핌핍핏핑하학한할핥함합핫항해핵핸핼햄햅햇했행햐향허헉헌헐헒험헙헛헝헤헥헨헬헴헵헷헹혀혁현혈혐협혓혔형혜혠혤혭호혹혼홀홅홈홉홋홍홑화확환활홧황홰홱홴횃횅회획횐횔횝횟횡효횬횰횹횻후훅훈훌훑훔훗훙훠훤훨훰훵훼훽휀휄휑휘휙휜휠휨휩휫휭휴휵휸휼흄흇흉흐흑흔흖흗흘흙흠흡흣흥흩희흰흴흼흽힁히힉힌힐힘힙힛힝갋갣걥겷괐괢굠굥궸귕귬긂긇긓깄깯꺆꺍껓껕꼉꼳꽅꽸꿘뀰뀼낻냗냡냣냬넏넢넫녇녱놁놑놰뇄뇡뇸눍눝뉻늗늧늼닁닏닽댠됭둗둚뒙딮딷똠똡똣똭똰뙇뙜뚧뜳뜽뜾랃랟랲럔럲럳렜렫롣롹뢔뤤맜맟맫먄몱뫠뫴뭥뮊뮹믁믕믜밷뱜뱡볌볻볿봥뵴붠붴뷁븡븨빋빧뺜뽓뾱뿕뿝쀠쁭샏샾섁섿셱솀솁솓쇵숖슌싥싳싿쎔쎠쎤쎵쎼쏼쑝쒐쒬씃씿앋앜얬얭옏옝옦옫왘왭왰욷웇웟웻윾읩읭읻잌잍쟵젇젉좬즒즤짣짲쫃쫒쬲쮓찓찟쵀췍칢칮칰칻캨캰컄켘콛쾃쿈쿽퀌퀜퀠큲킄탇턻톧퇻툶퉷팓팤팯펵퐉핰핳핻햏햔햣헗헠헡헣헿홥홨횽훕흝힣ㄱㄲㄳㄴㄵㄶㄷㄸㄹㄺㄻㄼㄽㄾㄿㅀㅁㅂㅃㅄㅅㅆㅇㅈㅉㅊㅋㅌㅍㅎㅏㅐㅑㅒㅓㅔㅕㅖㅗㅘㅙㅚㅛㅜㅝㅞㅟㅠㅡㅢㅣABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz1234567890 ,.<>/?;:'"[]{}\|`~-_=+!@#$%^&*()！ ＇ ， ． ／ ： ； ？ ＾ ＿ ｀ ｜ ￣ 、 。 · ‥ … ¨ 〃 ­ ― ∥ ＼ ∼ ´ ～ ˇ ˘ ˝ ˚ ˙ ¸ ˛ ¡ ¿ ː ‽ ⁂ ©＂ （ ） ［ ］ ｛ ｝ ‘ ’ “ ” 〔 〕 〈 〉 《 》 「 」 『 』 【 】＄ ％ ￦ Ｆ ′ ″ ℃ Å ￠ ￡ ￥ ¤ ℉ ‰ € ㎕ ㎖ ㎗ ℓ ㎘ ㏄ ㎣ ㎤ ㎥ ㎦ ㎙ ㎚ ㎛ ㎜ ㎝ ㎞ ㎟ ㎠ ㎡ ㎢ ㏊ ㎍ ㎎ ㎏ ㏏ ㎈ ㎉ ㏈ ㎧ ㎨ ㎰ ㎱ ㎲ ㎳ ㎴ ㎵ ㎶ ㎷ ㎸ ㎹ ㎀ ㎁ ㎂ ㎃ ㎄ ㎺ ㎻ ㎼ ㎽ ㎾ ㎿ ㎐ ㎑ ㎒ ㎓ ㎔ Ω ㏀ ㏁ ㎊ ㎋ ㎌ ㏖ ㏅ ㎭ ㎮ ㎯ ㏛ ㎩ ㎪ ㎫ ㎬ ㏝ ㏐ ㏓ ㏃ ㏉ ㏜ ㏆＃ ＆ ＊ ＠ § ※ ☆ ★ ○ ● ◎ ◇ ◆ □ ■ △ ▲ ▽ ▼ → ← ↑ ↓ ↔ 〓 ◁ ◀ ▷ ▶ ♤ ♠ ♡ ♥ ♧ ♣ ⊙ ◈ ▣ ◐ ◑ ▒ ▤ ▥ ▨ ▧ ▦ ▩ ♨ ☏ ☎ ☜ ☞ ¶ † ‡ ↕ ↗ ↙ ↖ ↘ ♭ ♩ ♪ ♬ ㉿ ㈜ № ㏇ ™ ㏂ ㏘ ℡ ® ª º ㉾─ │ ┌ ┐ ┘ └ ├ ┬ ┤ ┴ ┼ ━ ┃ ┏ ┓ ┛ ┗ ┣ ┳ ┫ ┻ ╋ ┠ ┯ ┨ ┷ ┿ ┝ ┰ ┥ ┸ ╂ ┒ ┑ ┚ ┙ ┖ ┕ ┎ ┍ ┞ ┟ ┡ ┢ ┦ ┧ ┩ ┪ ┭ ┮ ┱ ┲ ┵ ┶ ┹ ┺ ┽ ┾ ╀ ╁ ╃ ╄ ╅ ╆ ╇ ╈ ╉ ╊㉠ ㉡ ㉢ ㉣ ㉤ ㉥ ㉦ ㉧ ㉨ ㉩ ㉪ ㉫ ㉬ ㉭ ㉮ ㉯ ㉰ ㉱ ㉲ ㉳ ㉴ ㉵ ㉶ ㉷ ㉸ ㉹ ㉺ ㉻ ㈀ ㈁ ㈂ ㈃ ㈄ ㈅ ㈆ ㈇ ㈈ ㈉ ㈊ ㈋ ㈌ ㈍ ㈎ ㈏ ㈐ ㈑ ㈒ ㈓ ㈔ ㈕ ㈖ ㈗ ㈘ ㈙ ㈚ ㈛ⓐ ⓑ ⓒ ⓓ ⓔ ⓕ ⓖ ⓗ ⓘ ⓙ ⓚ ⓛ ⓜ ⓝ ⓞ ⓟ ⓠ ⓡ ⓢ ⓣ ⓤ ⓥ ⓦ ⓧ ⓨ ⓩ ① ② ③ ④ ⑤ ⑥ ⑦ ⑧ ⑨ ⑩ ⑪ ⑫ ⑬ ⑭ ⑮ ⒜ ⒝ ⒞ ⒟ ⒠ ⒡ ⒢ ⒣ ⒤ ⒥ ⒦ ⒧ ⒨ ⒩ ⒪ ⒫ ⒬ ⒭ ⒮ ⒯ ⒰ ⒱ ⒲ ⒳ ⒴ ⒵ ⑴ ⑵ ⑶ ⑷ ⑸ ⑹ ⑺ ⑻ ⑼ ⑽ ⑾ ⑿ ⒀ ⒁ ⒂０ １ ２ ３ ４ ５ ６ ７ ８ ９ ⅰ ⅱ ⅲ ⅳ ⅴ ⅵ ⅶ ⅷ ⅸ ⅹ Ⅰ Ⅱ Ⅲ Ⅳ Ⅴ Ⅵ Ⅶ Ⅷ Ⅸ X½ ⅓ ⅔ ¼ ¾ ⅛ ⅜ ⅝ ⅞ ¹ ² ³ ⁴ ⁿ ₁ ₂ ₃ ₄ㄱ ㄲ ㄳ ㄴ ㄵ ㄶ ㄷ ㄸ ㄹ ㄺ ㄻ ㄼ ㄽ ㄾ ㄿ ㅀ ㅁ ㅂ ㅃ ㅄ ㅅ ㅆ ㅇ ㅈ ㅉ ㅊ ㅋ ㅌ ㅍ ㅎ ㅏ ㅐ ㅑ ㅒ ㅓ ㅔ ㅕ ㅖ ㅗ ㅘ ㅙ ㅚ ㅛ ㅜ ㅝ ㅞ ㅟ ㅠ ㅡ ㅢ ㅣㅥ ㅦ ㅧ ㅨ ㅩ ㅪ ㅫ ㅬ ㅭ ㅮ ㅯ ㅰ ㅱ ㅲ ㅳ ㅴ ㅵ ㅶ ㅷ ㅸ ㅹ ㅺ ㅻ ㅼ ㅽ ㅾ ㅿ ㆀ ㆁ ㆂ ㆃ ㆄ ㆅ ㆆ ㆇ ㆈ ㆉ ㆊ ㆋ ㆌ ㆍ ㆎＡ Ｂ Ｃ Ｄ Ｅ Ｆ Ｇ Ｈ Ｉ Ｊ Ｋ Ｌ Ｍ Ｎ Ｏ Ｐ Ｑ Ｒ Ｓ Ｔ Ｕ Ｖ Ｗ Ｘ Ｙ Ｚ ａ ｂ ｃ ｄ ｅ ｆ ｇ ｈ ｉ ｊ ｋ ｌ ｍ ｎ ｏ ｐ ｑ ｒ ｓ ｔ ｕ ｖ ｗ ｘ ｙ ｚΑ Β Γ Δ Ε Ζ Η Θ Ι Κ Λ Μ Ν Ξ Ο Π Ρ Σ Τ Υ Φ Χ Ψ Ω α β γ δ ε ζ η θ ι κ λ μ ν ξ ο π ρ σ τ υ φ χ ψ ωÆ Ð Ħ Ĳ Ŀ Ł Ø Œ Þ Ŧ Ŋ æ đ ð ħ ı ĳ ĸ ŀ ł ø œ ß þ ŧ ŋ ŉぁ あ ぃ い ぅ う ぇ え ぉ お か が き ぎ く ぐ け げ こ ご さ ざ し じ す ず せ ぜ そ ぞ た だ ち ぢ っ つ づ て で と ど な に ぬ ね の は ば ぱ ひ び ぴ ふ ぶ ぷ へ べ ぺ ほ ぼ ぽ ま み む め も ゃ や ゅ ゆ ょ よ ら り る れ ろ ゎ わ ゐ ゑ を んァ ア ィ イ ゥ ウ ェ エ ォ オ カ ガ キ ギ ク グ ケ ゲ コ ゴ サ ザ シ ジ ス ズ セ ゼ ソ ゾ タ ダ チ ヂ ッ ツ ヅ テ デ ト ド ナ ニ ヌ ネ ノ ハ バ パ ヒ ビ ピ フ ブ プ ヘ ベ ペ ホ ボ ポ マ ミ ム メ モ ャ ヤ ュ ユ ョ ヨ ラ リ ル レ ロ ヮ ワ ヰ ヱ ヲ ン ヴ ヵ ヶА Б В Г Д Е Ё Ж З И Й К Л М Н О П Р С Т У Ф Х Ц Ч Ш Щ Ъ Ы Ь Э Ю Я а б в г д е ё ж з и й к л м н о п р с т у ф х ц ч ш щ ъ ы ь э ю я
```


**Weight**
---  

    ultralight = 100
    thin = 200
    light = 300
    normal = 400
    medium = 500
    bold = 700
    black/extrabold = 800

---


양식이 맞지 않아 통일하는데 커밋을 너무 많이 해버렸습니다 ㅜ  
최대한 여러브라우저에서 확인했지만, 간혹 변환기 오류로 확인이 안되는 경우가 발생합니다.  
피드백 주시면 개선하도록 하겠습니다.  



참고 URL
------
[onlinefontconverter](https://onlinefontconverter.com/)  
[nonria님의 블로그 - 웹 폰트로 사용하기 위한 서브셋 지정](https://nonria.com/post/96/)
