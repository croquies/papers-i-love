# 컴퓨터 과학 논문을 읽어야 합니다

| author(s)    | title                                                  | date          | link                                                                                                               |
|--------------|--------------------------------------------------------|---------------|--------------------------------------------------------------------------------------------------------------------|
| Ryan Donovan | You should be reading academic computer science papers | April 7, 2022 | [stackoverflow.blog](https://stackoverflow.blog/2022/04/07/you-should-be-reading-academic-computer-science-papers) |

현업 프로그래머로서 여러분은 계속 배울 필요가 있습니다. 튜토리얼, 문서, 스택오버플로우 질문 등, 찾을 수 있는 모든 것이 코드를 작성하고 실력을 최신 상태로 유지하는 데 도움을 줍니다. 하지만 프로그래밍 실력을 개선하기 위해 얼마나 자주 학술 논문을 찾아보나요?

튜토리얼은 지금 당장 코드를 작성할 수 있도록 도와주지만, 학술 논문은 프로그래밍이 어디에서 왔고, 어디로 향하는지 이해하도록 도와줍니다. 널 포인터([the billion dollar mistake](https://qconlondon.com/london-2009/qconlondon.com/london-2009/speaker/Tony+Hoare.html))부터 오브젝트([스몰토크](https://softwareengineering.stackexchange.com/questions/142327/what-did-they-call-object-oriented-programming-before-alan-kay-invented-the-term/142330#142330))에 이르기까지, 모든 프로그래밍 특성은 1960년대(혹은 더 이른 시기)까지 거슬러 올라가는 연구의 토대 위에 구축되었습니다. 미래의 혁신은 오늘날의 연구를 토대로 삼을 것입니다.

우리는 온라인 저장소를 운영하는 Papers We Love 팀의 멤버 중 세 명과 이야기를 나누어 보았습니다.

BlockFi 엔지니어링 디렉터 지샨 라카니(Zeeshan Lakhani), Datadog 엔지니어링 팀 리더 대런 뉴턴(Darren Newton), SageSure 엔지니어 데이비드 애쉬비(David Ashby)는 모두 Arc90이라는 회사에서 일하던 중 만났습니다. 이들 중 그 누구도 컴퓨터 과학에 대한 정규 교육을 받은 사람은 없었지만, 모두가 더 많은 것을 배우고 싶어 했습니다. 세 사람은 모두 인문학이나 예술을 전공했습니다. 애쉬비는 영문학을 전공하고 역사학을 부전공했으며, 뉴턴은 예술 학교에 두 번 다녔습니다. 라카니는 음악 및 음향 공학 석사 학위를 받기 전 영상대학원에 있었습니다. 이러한 학문 분야는 모두 실천의 기반이 되는 이론을 이해하기 위해, 학문의 기초를 세운 글을 읽는 것에 크게 의존하고 있습니다.

좋은 인문학도가 그러하듯, 세 사람은 아카이브에서 답을 찾기로 했습니다. 뉴턴은 말합니다. "제 안에 잠재된 사서가 있었어요. 그래서 저는 항상 제가 하는 일에 대한 역사적 자료에 관심이 많았죠."

## 역사 조사하기

프로그래밍의 역사에 대해 더 배우기 위해 애쉬비는 70년대 후반 32비트 마이크로컴퓨터를 설계하기 위한 경쟁에 관한 트레이시 키더(Tracy Kidder)의 책 "Soul of a New Machine"을 읽었습니다. 이 책은 당대의 엔지니어링 문화와 문제, 엔지니어들이 씨름하던 개념들에 대해 모두 다루고 있었습니다. 대량 판매 CPU와 표준 마더보드가 나오기 이전의 시대였기 때문에, 오늘날 우리가 당연하게 여기는 많은 것들이 막 해결되고 있던 시기였습니다.

세 사람은 키더의 책에서 컴퓨터 과학의 전체 역사를 볼 수 있었고, 이들은 기초적인 논문으로 1978년 출간된 [토니 호어(Tony Hoare)](http://www.cs.ox.ac.uk/people/publications/date/Tony.Hoare.html)의 "[Communicating Sequential Processes](https://www.cs.ox.ac.uk/files/6164/H76%20-%20Communicating.pdf)"를 읽어보기로 했습니다. 이들은 업무에 클로저와 클로저스크립트를 동시에 사용하고 있었기 때문에 이 논문이 적절해 보였습니다. 그런데 세 사람이 논문에 대해 논의하기 위해 모여 앉았을 때, 아무도 논문을 어떻게 이해해야 할지 모른다는 것을 깨달았습니다. 라카니는 "저는 이 논문의 절반밖에 이해할 수 없었지만, 도입부는 굉장히 좋아보였어요. 우리에게는 이걸 설명해줄 [데이비드 놀런(David Nolen)](https://github.com/readme/stories/david-nolen)같은 사람이 필요했어요."라고 말합니다.

놀런은 뉴욕 타임스에서 일하는 지인이었습니다. 그는 존 맥카시(John McCarthy)의 초기 논문을 인용하며 클로저와 Lisp-like 언어들에 대해 강연을 했습니다. 학문적 맥락과 함께 그의 설명을 듣자 세 사람의 마음 속에는 몇 가지 톱니바퀴를 돌기 시작했습니다. 바로 이때 Papers We Love라는 아이디어가 탄생했습니다.

우리가 매일 사용하는 컴퓨팅 개념의 역사를 알면 실제 수준에서 컴퓨터가 작동하는 방식에 대해 이해할 수 있습니다. 데이터베이스부터 프로그래밍 언어까지, 우리가 사용하는 도구들은 학술 연구에 기초하고 있습니다. 애쉬비는 "단순히 매일 사용하는 것만으로는 얻을 수 없는 지식이 있습니다. 그들이 걸어가지 않은 길을 이해하지 못하기 때문이죠. 하지만 여러분이 작업하는 것의 뿌리를 이해하면 그 지식을 얻을 수 있습니다."라고 말합니다.

세 사람이 좋아하는 브렛 빅터(Bret Victor)의 2013년 강연 "[The Future of Programming](https://www.youtube.com/watch?v=8pTEmbeENF4)"이 있습니다. 그는 70년대 엔지니어 같은 옷차림을 하고, 강연의 이름이 쓰인 프로젝터를 사용해 강연을 시작합니다. 그가 슬라이드를 조정하자 날짜가 1973년임을 알 수 있게 됩니다. 그는 연구로부터 나온 위대한 것들과 컴퓨터 과학을 뒤흔들만한 것들에 대해 이야기합니다. 모두 순차적 실행에서 동시성 모델로의 이동과 같이 청중들이 여전히 다루고 있는 것들입니다.

"중요한 건 오랜 시간이 걸렸다는 점입니다." 라카니는 말합니다. "오래된 것이 다시 새롭게 되고, 또 다시, 또 다시 새로워집니다." 문제가 생각보다 어렵기 때문인지, 아니면 그 문제에 대한 연구가 널리 공유되었기 때문인지, 과거와 동일한 문제들이 지금도 여전히 유의미합니다.

Papers We Love의 세 사람은 컴퓨팅 역사에 대한 사랑을 홀로 발견하지 않았습니다. 기술의 실천에 관해 더 배우기 위해 [과거의 시스템](https://retrocomputing.stackexchange.com/)에 대한 관심이 증가하고 있습니다. 이는 오래된 논문을 읽는 것의 또 다른 측면입니다. 여러분은 프로그래머들이 사용했던 오래된 하드웨어와 소프트웨어를 현재의 사고방식으로 사용합니다. 뉴턴은 "많은 사람들이 라즈베리파이에서 오래된 운영체제를 돌리고 있습니다. 라즈베리파이에서 오래된 스몰토크VM을 실행하거나 PDP-10을 다시 만드는거죠."라고 말합니다.

이러한 문제를 다루기 위해 노력한 연구 논문을 읽는 것과 같이, 초기 맥락에서 문제를 보면 지금 있는 자리에서 더 나은 관점이 생깁니다. "오브젝트는 80년대의 스몰토크로부터 만들어졌습니다. 이것은 큰 시스템들이 현재의 모습을 갖추게 된 이유입니다. 자바가 이런 모습을 갖게된 이유기도 하죠." 애쉬비가 말합니다.

새롭게 이해하는 것은 여러분이 직면한 문제를 해결하도록 도울 수 있습니다.

## 프로그래밍의 미래

연구 논문을 읽을 이유는 역사를 이해하는 것 외에도 더 있습니다. 현재의 논문을 읽음으로써 문제를 해결하는 새로운 방법을 찾을 수도 있습니다. 애쉬비는 말합니다. "스택오버플로우의 개념은 여러분의 문제를 다른 누군가가 이미 겪었다는 거죠. 학술 논문의 개념은 여러분의 문제를 다른 누군가가 이미 고민했다는 것입니다."

만약 여러분의 일이 오래된 [CRUD](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete) 앱의 변형을 만드는 것이라면, 아마 연구 논문이 도움을 주지 못할 것입니다. 하지만 여러분이 업계의 독특한 문제를 풀기 위해 노력하고 있다면 그 문제 공간에 있는 연구 중 일부가 도움을 줄 수 있을 것입니다. 애쉬비는 "저는 무엇이 가능한가에 대한 아이디어를 확장하기 위해 논문을 찾아봐요. 문제를 해결할 수 있는 다른 방법이 있다는 것을 이해하는데 도움을 받을 수 있거든요."라고 말합니다.

뉴턴과 데이터독의 동료들에게 학술 논문은 업무의 필수적인 부분입니다. 데이터독의 모니터링 소프트웨어는 애플리케이션의 상태와 스택에 대한 정보를 제공하기 위해 방대한 데이터를 실시간으로 처리합니다. 뉴턴은 "저희는 성능 알고리즘과 [대량의 통계 데이터를 처리하기 위한 더 나은 방법](https://blog.acolyer.org/2019/09/06/ddsketch/)에 많은 신경을 쓰고 있습니다. 우리는 그 중 일부를 학술 연구에 의존해야 합니다."라고 설명합니다.

물론 연구가 존재한다고 해서 여러분의 문제가 자동으로 해결되지는 않습니다. 때로는 하나의 논문이 해결책의 일부분만 제시하기도 합니다. 라카이는 "제가 Comcast에서 일할 때 라우팅 측면에서 로드밸런싱을 활용하고자 했습니다. 우리는 결국 서로 관련이 없는 세 종류의 논문을 적용했어요. 시맨틱을 네트워크 패킷에 담고, 특정 프로토콜을 통해 다른 논문의 내용을 기반으로 라우팅 시켰습니다. 많은 IETF 스펙을 구현했죠. 이 작업의 일부는 러스트 라이브러리로 만들어져 오늘날 사람들이 사용할 수 있게 되었습니다." 학술 논문에서 실마리를 찾아내 실제로 당면한 문제를 해결해낸 사례입니다.

논문을 읽지 않았다면 라카니의 팀은 효과적인 해결책을 설계하지 못했을 것입니다. 아니면 자체적인 방법을 찾았을지도 모르죠. 하지만 세 가지 개념을 연구하기 위한 작업의 양을 상상해보세요. 이미 연구가 된 작업이라면 같은 작업을 다시 할 필요가 없습니다. 거인의 어깨 위에 선다는 말처럼, 만약 여러분이 여러분의 분야에서 연구를 하고 있다면, 여러분은 어떤 거인의 어깨 위에 서야할지 정확히 알아야 합니다.

## 거인의 어깨에 관한 지도

저는 인문학도로서, 자연스럽게 누가 컴퓨터 과학의 거인인지 알고 싶어졌습니다. 만약 여러분이 인문학 스타일의 수업 커리큘럼을 만든다면 수업계획서에 넣을만한 논문들이죠. 앞으로 나아가기 위해 어떤 거인의 어깨 위에 설 수 있는지 알려주는 지도인 셈입니다.

컴퓨터 과학의 정석을 궁금해한 것은 제가 처음이 아니었습니다. 1996년 필립 파플란테(Phillip Laplante)가 "[Great Papers in Computer Science](https://www.google.com/books/edition/Great_Papers_in_Computer_Science/GmgZAQAAIAAJ?hl=en)"를 썼는데, 지금은 시대에 조금 뒤떨어졌을 수 있습니다. 같은 내용에 대한 보다 최근의 내용을 위해, 세 사람은 작년에 출간된 "[Ideas That Created the Future](https://mitpress.mit.edu/books/ideas-created-future)"를 추천합니다. 현재 카네기 멜론 대학교(제 모교)에서 컴퓨터 공학 박사과정을 밟고 있는 라카니는 처음엔 그 분야의 중요한 논문들을 다루는 과정이 있었다고 말합니다.

한편으로 컴퓨터 과학의 정석은 정확히 Papers We Love 저장소가 만들고자 하는 것입니다. 저장소에는 논문과 주제별로 정리된 논문 링크가 있습니다. 이 그룹은 여러분이 사랑하고, 주목받길 바라는 학술 논문에 대한 풀 리퀘스트를 환영합니다.

논문 읽기를 시작하고자 하는 누구나를 위해 여기 몇 개의 논문(그리고 강연들)을 추천합니다.

- [Dynamo: Amazon’s Highly Available Key-value Store](https://github.com/papers-we-love/papers-we-love/blob/f28b9c9f6c52a81aa9e60521c794f1c3aeafa9a7/datastores/dynamo-amazons-highly-available-key-value-store.pdf)
- [A Unified Theory of Garbage Collection](https://www.cs.cornell.edu/courses/cs6120/2019fa/blog/unified-theory-gc/)
- [Communicating Sequential Processes](http://www.cs.ucf.edu/courses/cop4020/sum2009/CSP-hoare.pdf)
- [Out of the Tar Pit](https://github.com/papers-we-love/papers-we-love/blob/f28b9c9f6c52a81aa9e60521c794f1c3aeafa9a7/design/out-of-the-tar-pit.pdf)

물론 더 많은 논문들도 있습니다.

만약 논문 읽기가 겁난다면, [Papers We Love의 발표](https://www.youtube.com/c/PapersWeLove/videos)를 확인해보세요. 논문을 이해하는 방법에 대한 지침이 될 것입니다. 이 발표는 논문에 대한 첫 번째 좌절을 다른 사람의 도움을 받아 해결하는 것에서 출발했습니다. 라카니는 "논문에 좌절했던 사람들이 클리프노트(_CliffsNotes_)를 받은거죠. 이제 그들은 논문을 공격할 수 있고, 제대로 이해할 수도 있습니다."라고 말합니다.

Paperes We Love 커뮤니티는 업계와 학계 사이에 다리를 놓기 위해 계속 노력하고 있습니다. 업계는 누군가 해결책을 구현하거나 오픈소스로 만들기 전에 새로운 해결책에 접근할 수 있고, 학계는 그들의 아이디어가 실제 상황에서 실험, 구현되는 것을 볼 수 있습니다. 이것은 모두에게 이익이 됩니다.

라카기는 말합니다. "Papers We Love의 목표 중 하나는 여러분이 자료를 조금 더 빠르게 찾을 수 있도록 만드는 것입니다. 그게 상황을 바꿀지도 모르죠."

