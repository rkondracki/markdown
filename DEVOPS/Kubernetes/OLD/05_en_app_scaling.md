복수의 앱 인스턴스를 구동하기
목표
kubectl을 사용해서 애플리케이션을 스케일한다.
애플리케이션을 스케일하기
지난 모듈에서 디플로이먼트, 를 만들고 서비스를 통해서 디플로이먼트를 외부에 노출시켜 봤다. 해당 디플로이먼트는 애플리케이션을 구동하기 위해 단 하나의 파드(Pod)만을 생성했었다. 트래픽이 증가하면, 사용자 요청에 맞추어 애플리케이션의 규모를 조정할 필요가 있다.

디플로이먼트의 복제 수를 변경하면 스케일링이 수행된다

요약:
디플로이먼트 스케일링하기
kubectl run 명령에 --replicas 파라미터를 사용해서 처음부터 복수의 인스턴스로 구동되는 디플로이먼트를 만들 수도 있다


스케일링 개요
 
이전다음
디플로이먼트를 스케일 아웃하면 신규 파드가 생성되어서 가용한 자원이 있는 노드에 스케줄된다. 스케일링 기능은 새로 의도한 상태(desired state)까지 파드의 수를 늘린다. 쿠버네티스는 파드의 오토스케일링 도 지원하지만 본 튜토리얼에서는 다루지 않는다. 0까지 스케일링하는 것도 가능하다. 이 경우 해당 디플로이먼트의 모든 파드가 종료된다.

애플리케이션의 인스턴스를 복수로 구동하게 되면 트래픽을 해당 인스턴스 모두에 분산시킬 방법이 필요해진다. 서비스는 노출된 디플로이먼트의 모든 파드에 네트워크 트래픽을 분산시켜줄 통합된 로드밸런서를 갖는다. 서비스는 엔드포인트를 이용해서 구동중인 파드를 지속적으로 모니터링함으로써 가용한 파드에만 트래픽이 전달되도록 해준다.

디플로이먼트의 복제 수를 변경하면 스케일링이 수행된다.


일단 복수의 애플리케이션의 인스턴스가 구동 중이면, 다운타임 없이 롤링 업데이트를 할 수 있다. 다음 모듈에서 이 내용을 다루도록 하겠다. 이제 온라인 터미널로 가서 애플리케이션을 스케일해보자.