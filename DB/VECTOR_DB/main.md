# Vector DB

<https://www.kdata.or.kr/info/info_04_view.html?field=&keyword=&type=techreport&page=49&dbnum=171604&mode=detail&type=techreport>

100배 빠른 데이터베이스 Vectorwise의 비밀

웹 시스템/단기 개발 프로젝트 매니지먼트

웹 애플리케이션의 개발을 성공시키려면 적절한 프로젝트 매니지먼트가 불가결하다. 그러나, 실제로는 프로젝트 매니지먼트 가 불충분하여 트러블이 끊이지 않고 있다. 개발 기간의 초과를 비롯하여 코스트 초과, 기능의 변경추가가 이어진다. 이 같 은 상황에서 고품질, 저코스트, 단기간의 개발 요구는 강해지고 있다.

속도한계 극복과 x86

대용량 데이터 시대를 맞이해 IBM, HP, 오라클, EMC, SAP 등 글로벌 IT 벤더가 적극적인 인수합병전략을 토대로 저마다 최고 성능의 데이터베이스를 선보이고 있다. 하드웨어에 최적화한 어플라이언스 형태의 제품을 내놓거나 소프트웨어 벤더는 하드웨어 업체와 손잡고 고성능 데이터베이스를 내놓고 있다. 오라클의 엑사데이터, IBM 네티자, EMC 그린플럼, SAP HANA가 국내에 비교적 일찍부터 알려진 것에 비해 ‘잉그레스’로 알려진 액티언이 선보인 벡터와이즈(Vectorwise)는 덜 알려졌다. 메인프레임과 유닉스를 거쳐 차세대 엔터프라이즈 컴퓨팅 플랫폼으로 떠오르는 x86을 발판으로 벡터와이즈가 어떤 기술과 전략으로 주무대에 등단할지 알아본다.

기회는 만들어가는 것

바야흐로 ‘데이터’를 둘러싸고 변화의 폭풍우가 몰아치고 있다. 급격한 변화 속에서는 많은 기회가 기다리고 있다. 기회를 잡으려면 변화를 보는 안목을 길러야 한다. 남다른 안목을 갖추지 못한 사람일지라도 ‘어떤 변화가 있을까?’ 하고 늘 생각하다 보면 기회를 잡을 확률은 그만큼 높아진다. 기회는 주어지는 것이 아니라 자신이 만드는 것이다.

DBMS를 비롯한 기존 소프트웨어는 폭발적인 데이터 증가와 최신 CPU 기술의 발전 속도를 추종할 수 없는 상황에 이르렀다. 이에 따라 대부분의 조직에서 데이터는 많지만 데이터 기반으로 중요한 결정을 내리지 못하는 상황이다. 벡터와이즈는 이 같은 문제점을 해결하기 위해 등장한 차세대 분석용 데이터베이스다.

새로운 데이터베이스 엔진을 사용해 일반 CPU에서도 최대의 성능을 도출한다. 벡터 기반의 처리와 온칩 메모리 기술을 활용해 기존 데이터베이스에 비해 높은 성능을 뽑아냄으로써 적게는 10배에서 최대 75배의 성능 향상을 가져왔다고 발표하고 있다. 저렴한 비용으로 신속하게 데이터를 검색하고 다양한 BI(Business Intelligence) 도구를 이용해 여러 방면에서 검색과 분석을 할 수 있게 한 것이다.

벡터와이즈는 성능 향상을 위해 고가의 유닉스 서버 대신에 범용 x86 서버에서 처리할 수 있다. 소프트웨어의 도입, 데이터 로드 최적화 명령, 검색 실행하는 간단한 절차로 구성됐다.

벡터와이즈의 특징

 ● 벡터 처리
 ● 칩의 캐시를 활용한 처리
 ● 업데이트 가능한 컬럼별 저장
 ● 자동으로 최적화한 압축
 ● 자동 인덱스
네덜란드 국립수학컴퓨터연구소에서 ‘X100’이라는 프로젝트가 진행됐다. 이 프로젝트의 목적은 ‘100배 빠른 데이터베이스를 만드는 것’이었다. 100배라는 목표를 설정한 계기는 ‘C 언어로 작성된 프로그램과 관계형 데이터베이스의 처리는 100배 정도의 차이가 난다’는 점에서 착안했다. 이 X100 프로젝트의 성과를 액티언(Actian)이 인수해 상용화한다. 이 액티언은 다름 아닌 ‘Ingres’ DB를 공급했던 바로 인그레스(Ingres Corporation)다. 90년대부터 DB 업계에서 일했던 사람이라면 낯설지 않은 이름이다. X100 프로젝트의 결과물로서 ‘100배 빠른 데이터베이스’를 목표로 태어난 것이 바로 ‘벡터와이즈’다.

컬럼형 분석 지원 BI 데이터베이스

벡터와이즈는 성능 향상을 위한 다양한 기술을 갖고 있다. 일반적인 RDB 성능은 스토리지 처리의 비효율성 때문에 저하된다. 그동안 RDB의 스토리지는 행 중심의 구조다. 이것은 OLTP 트랜잭션에서 효율은 좋지만, 분석 등에서는 적합하지 않다. 그래서 벡터와이즈는 스토리지의 구조를 분석 용도에 최적화해 컬럼형 구조로 접근했다.

디스크의 데이터 블록 크기도 크고, 성능이 최대화하도록 조정돼 있다. 모든 데이터 블록은 열마다 생성된 블록 내에 최소/최대 값을 갖고 있으며, 그것을 사용해 빠른 참조 처리를 한다. 또한 고속 메모리 버퍼를 디스크에 할당함으로써 속도를 높였다. 이 메모리 버퍼는 CPU 처리를 효율화하기 위해 디스크로부터 비동기적으로 데이터를 읽을 수 있다. 데이터의 압축을 적극 활용한다. 디스크뿐만 아니라 메모리에서도 압축해 CPU가 처리하는 데이터 크기를 줄인 것이다.

슈퍼컴퓨터에서 시작된 벡터 프로세싱

일반적인 조건에서 CPU는 한번에 1~2개의 데이터를 처리할 수 있다. 예를 들어 CPU에 ‘A와 B를 더한 후 결과를 C에 저장하라’는 명령을 내리면 A, B, C의 데이터는 바로 명령어에서 사용할 수 있도록 변환(encode)돼야 한다. 즉, 데이터가 저장된 메모리 위치의 주소를 지정하는(point to) 작업이 필요하다. 이처럼 주소를 디코딩하고 메모리에서 데이터를 가져오는 데는 일정한 시간이 걸린다. CPU 속도가 증가함에 따라 메모리 지연 시간(latency)이 성능에 큰 영향을 미치게 됐다.

이렇게 낭비되는 시간을 줄이기 위해 최근 CPU에서는 파이프라인 기술을 사용한다. 명령어는 몇 개의 서브 유닛을 차례로 통과한다. 첫 번째 서브 유닛에서는 어드레스를 읽어 해독하고 다음 서브 유닛은 주소 값을 불러오며(fetch), 그 다음 서브 유닛은 그것들을 연산한다. 파이프라인은 마치 조립 라인과 같이 CPU에서 하나의 명령이 끝나기 전에 다른 명령을 해독하기 시작하는 것으로 주소 디코더는 끊임없이 사용된다. 어떤 특정 명령어는 실행 완료되는 데 일정한 시간이 걸린다. 이 시간을 레이턴시라고 한다. CPU는 파이프라인을 이용해 레이턴시 동안 기다리지 않고 한번에 하나씩 실행할 수 있다.

벡터 프로세서는 이런 개념을 한층 발전시켜 명령어를 파이프라인하는 것만 아니라, 데이터 그 자체도 파이프라인으로 처리되도록 했다. A와 B를 더하라는 명령뿐만 아니라 지정한 범위 안의 모든 숫자를 더할 수 있도록 한 것이다. 즉, 한 컬럼의 모든 숫자를 다른 컬럼의 모든 숫자에 모두 더할 수 있다. 끊임없이 명령어를 해독하고 거기에 필요한 데이터를 가져오는 대신, 메모리는 한 번에 하나의 명령어로만 읽을 수 있는데 마지막 사용한 주소에서 하나 더 큰 주소가 다음에 필요한 주소다. 이 방법은 디코딩 시간을 줄이는 데 도움이 된다.
(출처: http://ko.wikipedia.org/wiki/벡터_프로세서)


execute this loop 10 times
read the next instruction and decode it
fetch this number
fetch that number
add them
put the result here
end loop read instruction and decode it
fetch these 10 numbers
fetch those 10 numbers
add them
put the results here
벡터와이즈는 내부적으로 스토리지 인덱스라는 것을 갖고 있어서 데이터베이스 인덱스가 필요 없다. 데이터베이스 측에서는 이 스토리지 인덱스의 존재를 의식하지 않는다. 예를 들어 SQL 문이 좋지 않아 느려질 경우 일반적으로 SQL을 튜닝하지만, 벡터와이즈는 SQL 튜닝이 필요 없다.

CPU의 벡터 처리를 통한 성능 향상

최근 CPU는 벡터 처리 기능을 기본으로 지원함에도 불구하고 전통적인 RDB는 이 기능을 활용하지 못하고 있다. 벡터 처리는 SIMD(Single Instruction Multiple Data) 명령어를 사용해 한 번에 여러 개의 데이터를 처리하는 것이다. 벡터와이즈는 벡터 처리를 최대한 활용함으로써 성능 향상을 실현했다.

 ● CPU 캐시: 최근 CPU는 MB 단위의 CPU 캐시를 제공하는데, 이 제품은 CPU 캐시에 맞게 벡터 처리하도록 설계함으로써 속도를 높였다.
 ● 컬럼별 저장 구조와 압축: 기존 데이터베이스는 행별 저장구조다. 이 경우 분석에 필요 없는 열이 있어도, 모든 컬럼을 로드해야 한다. 반면 이 제품은 컬럼별 저장 구조이기 때문에 분석에 필요 없는 열을 가져오지 않고 필요한 열만 가져온다. 이때 데이터는 자동으로 컬럼에 압축한다. 이는 압축률을 통해 해당 영역의 성능 향상을 높인 것이다


<그림 1> 컬럼 단위 처리 구조


<그림 2> CPU에서 벡터 처리

CPU 벡터 처리로 ‘성능 높여’

벡터와이즈는 CPU의 성능을 최대한 이용해 처리 속도를 높였다. 기존 DB는 CPU 사용량은 높은것에 비해 CPU를 최적으로 사용하지 못하는 구조라는 점을 염두에 둔 접근이다. 지금 기준으로 보면, 저용량의 낮은 CPU 성능을 고려해 설계된 것이다.

벡터와이즈는 현재의 CPU 성능을 최대한 활용하기 위해 벡터 처리를 한다. CPU 안에서 데이터를 벡터로 처리함으로써 시스템의 처리량을 극대화한 것이다. 하나의 명령으로 하나의 작업을 하는 것이 아니라, 1024의 처리를 동시에 할 수 있는 것이다. 또한 CPU의 캐시를 최적으로 활용하도록 설계됐기 때문에 데이터 처리 효율이 그만큼 올라간다. 액티언은 컬럼 DB 기술과 CPU의 효율적인 사용으로 데이터 웨어하우스(DW)나 분석, BI 전문 영역에서 기존 DB보다 최고 100배 이상의 속도를 낼 수 있다고 소개한다.

새로운 콘셉트의 DB지만, 튜닝이나 성능 최적적화를 위한 기술적 사항이 간단하다는 점도 벡터와이즈가 강점으로 내세우는 점이다. 이 제품의 SQL 처리는 잉그레스 DB를 캡처해서 한다. 이것은 MySQL이 스토리지 엔진을 대체해 사용하는 것과 마찬가지로, 응용 프로그램에서는 벡터와이즈를 마치 인그레스 DB처럼 취급하는 것이다.

벡터와이즈는 최적의 성능을 내기 위해 CPU 코어당 8GB 정도의 메모리를 권장한다. 스토리지는 물론 광대역 I/O가 유리하다. 더불어 RAID 구성에서 SSD를 채용하면 속도를 내기 쉽다. 하지만 적은 용량의 SSD를 적용하는 것보다 더 많은 메모리에 저장하는 하는 것이 성능을 내기 유리하다고 소개한다.

하둡과 연동 지원

벡터와이즈는 다양한 영역에 공급되고 있다. 소셜 미디어 서비스를 제공하는 기업에서 온라인 광고를 분석하는 용도로 적극 이용되고 있다고 한다. 소셜 미디어에서의 사용자 경험 정보를 벡터와이즈에서 분석하고 최적화하는 것이다. 소셜 미디어의 클릭 스트림 데이터를 일단 하둡(Hadoop) 파일 시스템에 넣어 데이터마트화한 다음, 이것을 분석하기 쉬운 형태로 정리한 후 벡터와이즈에서 분석하는 것이다. 기존의 일반적인 데이터 웨어하우스 형태로 이용될 수 있지만, 이처럼 하둡과 연계해 구성할 수 있다는 점도 눈길을 끈다.

B2C 기업에서도 성공 사례도 소개하고 있다. 데이터 웨어하우스를 장기간 사용함에 따라 데이터 용량이 늘어나고, 이것이 성능 저하로 이어지면서 사용자 불만으로 표출되고 있다. 증가하는 데이터 수용을 위해 서버와 스토리지를 추가 도입함에 따른 TCO(총소유비용)가 증가할 수밖에 없는 것이 데이터 분석 시스템이 갖고 있는 특징이다. 성능은 떨어지고 TCO는 증가할 수밖에 없는 기존 분석 환경에서 저렴하면서 속도를 높일 수 있는 방법이 있다면, 그것은 단비와 같은 소식이 될 것이다. 이런 어려움을 안고 있는 곳에서 고가의 하드웨어로 업그레이드하는 대신 소프트웨어 측면에서 속도를 올릴 수 있는 방안 가운데 하나가 바로 CPU 캐시를 활용하는 벡터와이즈 DBMS다.

스트림 데이터 분석용으로도 각광

스마트미터나 M2M, 로그 데이터 등 자동으로 생성된 대용량 데이터 분석에 대한 관심이 늘어나고 있다. 현재로선 데이터 양이 너무 많기 때문에 분석할 엄두도 내지 못한 곳이 적지 않다. 이런 사이트에서 벡터와이즈는 하나의 대안이 될 수 있다. 결국 벡터와이즈가 당장 적용할 수 있는 빅터이터용 DB라는 뜻이다. 쿼리 성능이 높기 때문에 분석 환경에서 성능 문제, 또는 사용자 확장성 문제를 안고 있는 같은 사용자라면 벡터와이즈를 주목할 필요가 있다. (자료 출처: http://www.vw-kr.com, http://www.actian.com)