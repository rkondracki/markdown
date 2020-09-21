
글래스 글래스 테이블 테이블 Splunk Enterprise Security에서에서 글래스 글래스 테이블 테이블 만들기 만들기 글래스 테이블을 만들어 환경의 보안 상태를 시각화하고 모니터링합니다. 사용자가 설계하는 백그라운드에 따라 실시간으로 업데이트되는 핵심 지표 같은 보안 메트릭이나 임시 검색을 추가할 수 있습니다.
1. Splunk Enterprise Security 메인 메뉴에서 글래스 글래스 테이블을 테이블 클릭합니다. 2. 새 글래스 글래스 테이블 테이블 만들기를 만들기 클릭합니다. 3. 새 글래스 테이블의 제목제목 및 설명설명을 입력하고 해당 테이블에 대한 권한권한을 설정합니다. 4. 글래스 글래스 테이블 테이블 만들기를 만들기 클릭하여 글래스 테이블을 만듭니다.
보안 이용 사례의 맥락에서 글래스 테이블을 설정하는 방법에 대한 설명은 글래스 테이블을 사용하여 환경 내 위협 활동 모 니터링을 참조하십시오.
글래스 글래스 테이블 테이블 시각화 시각화 작성작성
글래스 테이블 편집기의 유연한 캔버스와 편집 도구를 사용하여 글래스 테이블을 만듭니다.
1. 글래스 테이블 리스트에서 글래스 테이블 이름을 클릭합니다. 2. 편집 도구를 사용하여 이미지를 업로드하고, 도형을 그리고, 아이콘을 추가하고, 텍스트를 추가하고, 메트릭의 상호 관
계를 나타내도록 연결합니다. 3. 보안 메트릭 패널에서, 메트릭을 클릭하여 추가할 수 있는 핵심 지표 검색 위젯을 봅니다. 필요한 위젯이 보이지 않는
경우, ES 관리자가 새 핵심 지표 검색을 만들 수 있습니다. Splunk Enterprise Security 관리에서 Splunk Enterprise Security에서 핵심 지표 만들기 및 관리를 참조하십시오. 4. 핵심 지표 검색 위젯을 하나 이상 클릭하여 그리기 캔버스로 끌어 옮깁니다.
실시간으로 계속 업데이트되는 관련 검색 값이 표시된 위젯이 캔버스에 나타납니다. 자세한 내용은 위젯 설정을 참조 하십시오. 5. 위젯을 더 추가하여 시각화의 동적 요소를 확장합니다. 6. 임시임시 검색검색을 클릭하고 그리기 캔버스로 끌어 옮겨 검색 결과를 표시하는 사용자 지정 위젯을 추가합니다. 자세한 내용
은 검색 위젯 만들기 및 설정을 참조하십시오. 7. 저장저장을 클릭합니다.
위젯위젯 설정설정
위젯을 글래스 테이블에 추가한 후 설정하여 성능을 최적화하고, 사용자 지정 드릴다운을 추가하고, 특정 글래스 테이블 디 자인의 위젯 모양을 사용자 지정합니다. 핵심 지표 검색은 글래스 테이블에 포함된 위젯을 채웁니다. 콘텐츠 관리 대시보드 에서 핵심 지표 검색을 변경하십시오.
1. 글래스 테이블 편집기에서 위젯을 클릭합니다. 2. 사용자 사용자 지정지정 드릴다운에서 드릴다운 켜짐켜짐을 클릭합니다. 3. 드릴다운 대상을 선택하거나 URL을 입력합니다. 4. 시각화 시각화 유형유형에서 검색 결과를 표시하는 데 적절한 옵션을 선택합니다. 시각화 유형은 단일 값, 게이지, sparkline 및 단
일 값 델타 등입니다. 5. 업데이트를 업데이트 클릭하여 위젯 설정을 업데이트합니다. 6. 저장저장을 클릭합니다.
핵심 지표 검색 값은 핵심 지표 검색을 만들 때 정의하는 검색 일정에 따라 정기적인 간격으로 업데이트됩니다.
검색검색 위젯위젯 만들기 만들기 및 설정설정
검색 결과를 표시할 사용자 지정 위젯도 만들 수 있습니다. 다양한 시각화 유형을 사용하여 새 검색을 글래스 테이블에 추가 하고, 사용자 지정 검색 문자열을 정의하고, 검색 위젯의 모양을 사용자 지정하십시오.
사용자 지정 검색을 글래스 테이블 밖에서 작성하여 기대한 결과가 얻어지는지 확인하십시오. 임계값을 사용하려면 사용자 지정 검색에
timechart
명령어 또는
stats by _time
이 포함되어야 합니다.
1. 글래스 테이블 편집기에서 임시임시 검색검색을 클릭하여 캔버스로 끌어 옮깁니다. 2. 설정설정 패널에서, 검색검색 유형유형에 사용자 지정 검색 문자열을 입력합니다. 3. 시간 선택기를 사용하여 검색 종료 시간을 선택합니다. 기본값은 지금지금입니다. 4. 시작시작 시간시간 메뉴에서 검색 시작 시간을 선택합니다. 그러면 검색의 시작 시간이 시간 선택기에서 설정한 종료종료 날짜날짜 및
시간시간에 대해 상대적으로 결정되고, 검색이 적용되는 시간 범위가 결정됩니다. 보안 메트릭은 기본적으로 이전 48시간 의 결과를 표시합니다. 예를 들어 시간 범위 선택기를 지금지금으로 설정하면 보안 메트릭이 이전 48시간을 검색하고 결과를 표시합니다. 시간 범 위 선택기를 6시간시간 전으로 변경하면 보안 메트릭이 -54시간부터 -6시간까지의 결과를 표시합니다. 5. 임계값 임계값 필드필드에 검색의 임계값으로 사용할 필드를 입력합니다.
예: count
24
6. 임계값에 임계값 대해 켜짐켜짐을 클릭하여 검색 위젯에서 임계값을 활성화합니다. 7. 편집편집을 클릭하여 임계값을 편집합니다. 8. 임계값 창에 검색 위젯에 사용할 임계값을 추가합니다. 그러면 메트릭의 현재 상태를 나타내는 위젯의 색이 결정됩니
다. 9. 검색 위젯의 시각화 시각화 유형유형을 선택합니다. 10. 업데이트를 업데이트 클릭하여 위젯을 새 시각화로 업데이트하고 지정된 시간 범위의 검색 결과를 표시합니다. 11. 저장저장을 클릭합니다.
Splunk Enterprise Security에서에서 글래스 글래스 테이블 테이블 관리관리
글래스 테이블을 사용하여 환경의 보안 메트릭을 유연한 방법으로 시각화할 수 있습니다. Splunk Enterprise Security에 포 함된 글래스 테이블과 직접 만드는 글래스 테이블을 글래스 테이블 리스트 페이지에서 관리하십시오.
글래스 테이블 리스트 페이지에 접근하려면 Splunk Enterprise Security 메뉴 모음에서 글래스 글래스 테이블을 테이블 클릭하십시오.
글래스 글래스 테이블 테이블 수정수정
글래스 테이블을 만든 후 계속 변경할 수 있습니다.
1. 글래스 테이블 리스트에서 수정할 글래스 테이블 옆의 편집편집을 클릭합니다. 2. 글래스 테이블 자체를 편집할지, 제목이나 설명을 편집할지, 아니면 권한을 편집할지 선택합니다.
앱의앱의 일부로 일부로 가져온 가져온 후 삭제한 삭제한 글래스 글래스 테이블 테이블 복원복원
글래스 테이블을 앱의 일부로 가져온 후 나중에 삭제한 경우, 글래스 테이블을 다시 가져와서 복원할 수 없습니다. 대신 다음 작업을 수행하십시오.
1. 글래스 테이블을 가져온 앱을 비활성화합니다. 2. 앱 가져오기 프로그램이 실행될 때까지 몇 분 기다립니다. 3. 앱을 활성화합니다.
글래스 테이블이 다시 표시됩니다.
글래스 글래스 테이블을 테이블을 복제하여 복제하여 템플릿 템플릿 만들기 만들기 글래스 테이블을 복제하여 템플릿을 만들거나, Splunk Enterprise Security에 포함된 글래스 테이블을 원본으로 보존하고 다른 버전을 실험적으로 변경할 수 있습니다.
1. 글래스 테이블 리스트에서 수정할 글래스 테이블 옆의 편집편집을 클릭합니다. 2. 복제복제를 클릭합니다. 3. 새 제목을 입력합니다. 4. (선택 사항) 새로운 설명을 입력합니다. 5. (선택 사항) 복제된 글래스 테이블의 권한을 변경합니다. 6. 페이지 페이지 복제복제를 클릭합니다.
글래스 글래스 테이블 테이블 액세스 액세스 모든 사용자가 글래스 테이블을 볼 수 있지만, 글래스 테이블을 만들고 수정하려면 ess_analyst, ess_admin, 또는 관리자 역할이 있거나 "글래스 테이블 편집" 기능이 있어야 합니다. 필요한 권한이 없는 경우 Splunk Enterprise Security 관리자에 게 문의하십시오.
글래스 글래스 테이블에 테이블에 사용사용 가능한 가능한 검색검색
개별 글래스 테이블에서 만드는 임시 검색 위젯을 다른 글래스 테이블과 자동으로 공유할 수 없습니다. 핵심 지표 검색은 미 리 정의된 위젯으로 추가할 수 있는 보안 메트릭의 리스트를 채웁니다. ES 관리자는 콘텐츠 관리 페이지에서 핵심 지표 검색 을 만들고 편집할 수 있습니다. Splunk Enterprise Security에서 핵심 지표 검색 만들기 및 관리를 참조하십시오.
글래스 글래스 테이블 테이블 성능성능 및 저장저장
글래스 테이블 콘텐츠는 KV 스토어에 저장됩니다. 글래스 테이블 정의는
SplunkEnterpriseSecuritySuite_glasstables
컬렉 션에 저장됩니다. 글래스 테이블에 추가되는 이미지 같은 파일은
SplunkEnterpriseSecuritySuite_files
컬렉션에 저장됩니 다. 글래스 테이블에 추가하는 사용자 지정 위젯, 이미지 및 기타 항목이 모두 이 컬렉션에 저장됩니다.
개별 글래스 테이블의 성능은 글래스 테이블에 있는 검색 위젯 수에 좌우됩니다. 글래스 테이블을 보기 위해 열면 각 검색이 동시에 실행됩니다. 검색 위젯이 200개 이상인 글래스 테이블에 데이터가 표시되려면 10-15초 정도 걸릴 수 있습니다.
글래스 글래스 테이블 테이블 내보내기
내보내기 25
글래스 테이블을 내보내 다른 사람과 공유하거나 백업할 수 있습니다. Splunk Enterprise Security 관리에서 Splunk Enterprise Security에서 콘텐츠를 앱으로 내보내기를 참조하십시오.
26