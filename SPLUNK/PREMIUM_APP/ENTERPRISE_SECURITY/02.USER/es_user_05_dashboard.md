대시보드 대시보드 개요개요
Splunk Enterprise Security에서에서 사용사용 가능한 가능한 대시보드 대시보드 소개소개
Splunk Enterprise Security에는 보안 인시던트를 확인 및 조사하고, 이벤트에 담긴 심층 정보를 드러내고, 인시던트 조사 속도를 높이고, 다양한 보안 도메인의 상태를 모니터링하고, 인시던트 조사와 ES 배포를 감사(audit)하기 위한 대시보드가 100개 넘게 포함되어 있습니다.
가장 유용한 구체적인 대시보드는 Splunk Enterprise Security를 어떻게 사용할 계획인지에 따라 다릅니다.
보안보안 인시던트 인시던트 식별식별 및 조사조사
여러 대시보드 및 워크플로를 사용하여 보안 인시던트를 식별하고 조사할 수 있습니다. Splunk Enterprise Security는 상관상관 (correlation) 검색검색을 사용하여 환경의 보안 인시던트를 나타내는 주요주요 이벤트 이벤트를 식별합니다.
보안 포스처는 지난 24시간 동안 환경에서 발생한 주요 이벤트에 대한 개괄적인 개요를 제시합니다. 인시던트가 가장 많은 보안 도메인과 최근 작업을 식별할 수 있습니다. 보안 포스처 대시보드를 참조하십시오. 인시던트 검토에는 환경에서 식별된 모든 주요 이벤트의 세부 정보가 표시됩니다. 이 대시보드에서 주요 이벤트를 분 류 및 배정하고 주요 이벤트의 세부 정보를 검토하십시오. 인시던트 검토를 참조하십시오. 내 조사에는 환경의 모든 조사가 표시됩니다. 조사를 열고 조사 작업을 수행하여 진행 상황과 작업을 추적하면서 여러 관련 보안 인시던트를 조사할 수 있습니다. 내 조사를 참조하십시오.
보안보안 인텔리전스를 인텔리전스를 사용하여 사용하여 조사조사 속도속도 높이기 높이기
몇 가지 보안 인텔리전스 대시보드에서 특정 유형의 인텔리전스를 사용해 인시던트를 조사할 수 있습니다.
위험 분석은 네트워크 전역에 있는 시스템 및 사용자의 위험 점수를 평가하고 환경에 위협을 제기하는 특별히 위험한 장치와 사용자를 식별하기 위해 사용할 수 있습니다. 위험 분석을 참조하십시오. 프로토콜 인텔리전스 대시보드는 스트림 캡처 앱의 패킷 캡처 데이터를 사용하여 보안 조사와 관련된 네트워크에 대한 심층 정보를 제공합니다. 의심스러운 트래픽, DNS 작업, 이메일 작업을 식별하고, 네트워크 트래픽에서 사용 중인 연 결과 프로토콜을 검토합니다. 프로토콜 인텔리전스 대시보드를 참조하십시오. 위협 인텔리전스 대시보드는 Splunk Enterprise Security에 포함된 위협 인텔리전스 소스와 직접 설정하는 사용자 지 정 소스를 사용해 보안 인시던트에 컨텍스트를 부여하고 환경에서 알려진 악의적인 행위자를 식별합니다. 위협 인텔리 전스 대시보드를 참조하십시오. 사용자 인텔리전스 대시보드는 환경에서 사용자 및 자산의 작업을 조사하고 모니터링하는 데 사용할 수 있습니다. Asset 및 Identity Investigator 대시보드와 사용자 작업 모니터링을 참조하십시오. 웹 인텔리전스 대시보드는 네트워크의 웹 트래픽을 분석하고 주요 HTTP 범주, 사용자 에이전트, 새 도메인 및 긴 URL을 식별하는 데 도움이 됩니다. 웹 인텔리전스 대시보드를 참조하십시오.
보안보안 도메인 도메인 작업작업 모니터링 모니터링
Splunk Enterprise Security와 함께 제공되는 도메인 대시보드는 중요한 보안 도메인의 이벤트와 상태를 모니터링하는 데 사용할 수 있습니다. 메인 대시보드에 요약된 데이터를 검토하고, 특정 도메인 검색 대시보드를 사용하여 원시 이벤트를 조 사할 수 있습니다.
액세스 도메인 대시보드에는 로그인 시도, 액세스 제어 이벤트 및 기본 계정 작업 같은 인증 및 액세스 관리 데이터가 표시됩니다. 액세스 대시보드를 참조하십시오. Endpoint 도메인 대시보드에는 멀웨어 감염과 관련된 endpoint 데이터, 패치 이력, 시스템 설정 및 시간 동기화 정보 가 표시됩니다. Endpoint 대시보드를 참조하십시오. 네트워크 도메인 대시보드에는 방화벽, 라우터, 네트워크 침입 탐지 시스템, 네트워크 취약성 스캐너, 프록시 서버 및 호스트 같은 장치에서 제공한 네트워크 트래픽 데이터가 표시됩니다. 네트워크 대시보드와 웹 센터 및 네트워크 변경 사항 대시보드와 포트 & 프로토콜 추적기 대시보드를 참조하십시오. ID 도메인 대시보드에는 자산 및 ID 리스트의 데이터와 사용 중인 세션 유형이 표시됩니다. 자산 및 ID 대시보드를 참 조하십시오.
보안보안 메트릭 메트릭 시각화 시각화
글래스 테이블을 만들어 환경의 보안 메트릭을 시각화합니다. 환경 내 위협 활동을 모니터링하거나, Splunk Enterprise Security 배포의 상태를 평가하거나, 공격자가 네트워크에서 이동한 경로를 매핑하여 공격자의 향후 침입 시도를 모니터링 할 수 있습니다. 글래스 테이블 만들기를 참조하십시오.
Splunk Enterprise Security의 감사감사(audit) 작업작업
감사(audit) 대시보드는 Splunk Enterprise Security에 의해 수행되는 백그라운드 프로세스와 작업에 대한 심층 정보를 제 시합니다. 일부 감사(audit) 대시보드에서는 Splunk Enterprise Security에서 사용자가 수행한 작업을 검토할 수 있는 한편, 배포 환경과 데이터 모델 및 콘텐츠 사용 상태에 대한 심층 정보를 부여하는 대시보드도 있습니다. 감사(audit) 대시보드를 참조하십시오.
27
이용이용 사례에 사례에 맞게맞게 Splunk Enterprise Security 대시보드 대시보드 사용자 사용자 지정지정
대시보드와 대시보드 패널에 사용되는 검색을 변경하여 조직, 환경 또는 보안 이용 사례와 관련성이 더 높은 검색을 만들 수 있습니다. 대시보드 패널에 사용되는 검색을 패널 편집기로 보고 데이터가 어디서 오는지 확인하십시오. 패널과 패널에 사용 되는 검색은 물론 시각화의 제목도 편집할 수 있습니다.
Splunk Enterprise의 경우, Splunk Enterprise 대시보드 및 시각화에서 대시보드 편집기로 대시보드 편집을 참조하 십시오. Splunk Cloud의 경우, Splunk Cloud 대시보드 및 시각화에서 대시보드 편집기로 대시보드 편집을 참조하십시오.
원시원시 이벤트로 이벤트로 드릴다운 드릴다운
원시 이벤트까지 드릴다운하여 대시보드에 있는 데이터를 더 깊이 파고 들고, 워크플로 작업을 사용해 원시 이벤트를 뛰어넘 어 대시보드의 특정 필드를 조사하거나 Splunk 플랫폼 밖에서 다른 작업을 수행할 수 있습니다.
대시보드의 차트와 테이블에서 원시 이벤트까지 드릴다운할 수 있습니다. 드릴다운 동작에 대한 내용은 Splunk 플랫폼 매뉴 얼에서 확인할 수 있습니다.
Splunk Enterprise의 경우 Splunk Enterprise 대시보드와 시각화의 대시보드 상호작용에 드릴다운 사용을 참조하십 시오. Splunk Cloud의 경우 Splunk Cloud 대시보드와 시각화의 대시보드 상호작용에 드릴다운 사용을 참조하십시오.
사용자 사용자 지정지정 워크플로 워크플로 작업작업 만들기 만들기
워크플로 작업을 사용하여 원시 이벤트에 대해 작업을 수행할 수 있습니다. 사용자 지정 워크플로 작업도 만들 수 있습니다. 워크플로 작업에 대한 내용은 Splunk 플랫폼 매뉴얼에서 확인할 수 있습니다.
Splunk Enterprise의 경우, Splunk Enterprise 지식 관리자 매뉴얼에서 워크플로 작업이 필드 및 이벤트 메뉴에 표시 되는 방법 제어를 참조하십시오 Splunk Cloud의 경우 Splunk Cloud 지식 관리자 매뉴얼에서 워크플로 작업이 필드 및 이벤트 메뉴에 표시되는 방법 제어를 참조하십시오
Splunk Enterprise Security의 핵심핵심 지표지표
Splunk Enterprise Security에는 Splunk Enterprise Security에서 다루는 보안 도메인에 대한 핵심 보안 지표를 식별하는 미리 정의된 핵심 지표가 포함되어 있습니다. 핵심 지표를 Splunk Enterprise Security의 대시보드에서 보거나, 사용자 지정 글래스 테이블에 보안 메트릭으로 추가할 수 있습니다.
핵심 지표는 여러 보안 메트릭에 대한 시각적 기준을 제시합니다. 핵심 지표 검색은 핵심 지표의 보안 메트릭을 채웁니다. 핵 심 지표 검색은 Enterprise Security에서 정의된 데이터 데이터 모델모델이나 CIM(Common Information Model) 앱에서 정의된 데이 터 모델을 대상으로 실행됩니다. 일부 핵심 지표 검색은 주요주요 이벤트 이벤트 수에 대해 실행됩니다.
대시보드에서 대시보드에서 핵심핵심 지표지표 해석해석
대시보드에서, 각 핵심 지표에는 값 지표, 추세량, 추세 표시기, 그리고 지표의 중요도나 우선순위를 나타내는 데 사용되는 임 계값이 포함됩니다. 핵심 지표 검색은 기본적으로 48시간의 상대상대 시간시간 동안 실행됩니다.
필 드
설명설명
설 명
보안 관련 메트릭에 대한 간략한 설명
값 지 표
현재 이벤트 수. 임계값이 설정된 경우, 수가 임계값을 지나면 색상이 변경됩니다. 값 지표를 클릭하여 핵심 지표 검 색을 드릴다운하고 원시 이벤트를 봅니다. 100%보다 큰 백분율 값처럼 값 지표가 잘못된 경우, 핵심 지표 검색에서 값을 계산하기 위해 사용한 데이터 모델 데이터 집합에 누락되거나 잘못된 데이터가 있기 때문일 수 있습니다.
추 세 량
핵심 지표 검색에서 정의된 기간 동안의 이벤트 수 변동을 표시합니다.
28
추세 방향을 나타내는 방향 화살표를 표시합니다. 시간이 지남에 따라 화살표 색과 방향이 바뀝니다.
대시보드에서 대시보드에서 핵심핵심 지표지표 편집편집
Enterprise Security에는 미리 설정된 핵심 지표가 포함되어 있습니다. 각 대시보드 핵심 지표 행에는 대시보드에서 나가지 않고 주요 지표를 간단하게 시각적으로 변경하기 위해 사용할 수 있는 편집기가 있습니다. 핵심 지표를 생성하는 검색을 콘 텐츠텐츠 관리관리 대시보드에서 변경할 수 있습니다. Splunk Enterprise Security 관리에서 핵심 지표 검색 편집을 참조하십시오.
1. 지표 모음의 왼쪽 상단에 있는 편집편집 연필 아이콘을 클릭합니다. 편집 도구가 지표 위에 표시됩니다.
2. 지표를 끌어 옮겨서 재정렬합니다. 한 행에 지표가 5개까지 있을 수 있고, 여러 지표 행이 있을 수 있습니다. 3. 체크 표시 아이콘을 클릭하여 저장합니다.
대시보드에서 대시보드에서 핵심핵심 지표지표 제거제거
대시보드에서 핵심 지표를 제거하십시오.
1. 지표 모음의 왼쪽 상단에 있는 편집편집 연필 아이콘을 클릭합니다. 편집 도구가 지표 위에 표시됩니다.
2. 지표의 오른쪽 상단에 있는 X를 클릭합니다. 3. 체크 표시 아이콘을 클릭하여 저장합니다.
지표를 대시보드에서 제거해도 Enterprise Security에서 핵심 지표가 제거되지 않습니다.
대시보드에 대시보드에 핵심핵심 지표지표 추가추가
대시보드에 핵심 지표를 추가합니다.
1. 지표 모음의 왼쪽 상단에 있는 편집편집 연필 아이콘을 클릭합니다. 편집 도구가 지표 위에 표시됩니다.
2. 더하기 부호를 클릭하여 지표지표 추가추가 패널을 엽니다. 3. 체크 표시 아이콘을 클릭하여 저장합니다.
대시보드에서 대시보드에서 핵심핵심 지표지표 임계값 임계값 설정설정
대시보드에서 핵심 지표의 색이 변하는 임계값을 설정할 수 있습니다. 임계값은 지표 이벤트 수의 허용 값을 정의합니다. 이 벤트 수가 임계값을 초과하면 핵심 지표가 빨간색으로 표시되는 한편, 이벤트 수가 임계값보다 낮으면 핵심 지표가 녹색으로 표시됩니다. 임계값이 정의되지 정의되지 않음않음인 경우 이벤트 수가 검정색으로 유지됩니다.
1. 지표 모음의 왼쪽 상단에 있는 편집편집 연필 아이콘을 클릭합니다. 편집 도구가 지표 위에 표시됩니다.
29
추 세 표 시 기
2. 핵심 지표의 임계값 임계값을 입력합니다. 3. 체크 표시 아이콘을 클릭하여 저장합니다.
30