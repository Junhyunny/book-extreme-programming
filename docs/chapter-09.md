
## 9. 보조 실천방법

보조 실천방법은 기본 실천방법들을 완전히 하기 전에는 실행하기 어렵거나 실행하면 위험한 실천방법들이다. 
기본 실천방법들을 잘 실천하고 있다면 도전해보라. 

### 9.1. 진짜 고객 참여

시스템에 따라 인생과 사업이 달라지는 사람들을 팀의 일원이 되게 한다. 
고객 참여의 핵심은 필요를 느끼는 사람들(고객)에게 그 필요를 채워줄 수 있는 사람(우리)들과 직접 연결시켜 낭비를 없애는 것이다. 
고객은 우리가 기쁘게 만들려는 사람들이다. 
진짜 고객이 사용하지 않을 기능들을 개발하고, 테스트를 작성하는 일은 낭비가 될 수 있다. 
고객의 필요와 개발 능력의 거리가 가까울수록 프로젝트의 가치가 올라간다. 

### 9.2. 점진적 배치

큰 배치는 위험도 높고 인간적, 경제적으로 비용도 많이 든다. 

* e.g. 레거시 시스템을 교체하는데 빅뱅(bigbang)처럼 일괄적인 변경

당장 다룰 수 있는 작은 기능이나 제한된 데이터 집합을 하나 찾아서 시작해라. 
배치를 시작해라. 
그리고 레거시 시스템과 변경되는 시스템을 모두 돌릴 수 있는 방법을 찾는다. 

### 9.3. 팀 지속성

효율적인 팀은 계속 함께 일하도록 만든다. 
소프트웨어의 가치는 사람들이 아는 것과 하는 것뿐 아니라 인간관계와 사람들이 함께 성취하는 것을 통해서도 만들어진다. 
사람들이 자기가 알고 신뢰하는 사람들과 함께 일하도록 해주는 것은 가치있다. 

안정된 팀을 아예 변경하지 말라는 이야기는 아니다. 
대체로 팀을 유지하고 적정한 수준으로 회전하도록 장려하는 것은 안정된 팀이 내놓는 이익, 지식과 겸험의 전수를 모두 얻을 수 있다. 

### 9.4. 팀 크기 줄이기

팀의 능력이 신장되면, 작업량은 일정하게 유지하고 팀의 크기를 줄여서 더 많은 팀을 만든다. 

* e.g. 도요타 생산 시스템(TPS, Toyota Production System)

### 9.5. 근본 원인 분석

개발 후 결함이 발견되면 그 결함과 원인을 모두 제거한다. 
팀이 같은 실수를 저지르지 않도록 만든다. 

##### XP의 결함 대응 절차

1. 결함을 드러내는 시스템 차원의 자동화된 테스트를 작성한다. 
1. 결함을 드러내는 일에는 우리가 바라는 행동을 보여주는 일도 포함된다. 
1. 결함을 재생산하는 가능한 범위가 가장 좁은 단위 테스트를 작성한다.
1. 단위 테스트가 통과하도록 시스템을 고친다.
1. 테스트에 실패하면 3번으로 돌아간다.
1. 결함을 해결한 후에는 다음과 같은 것들을 확인한다.
    * 왜 이 결함이 생겼는지?
    * 왜 결함이 이전에 잡히지 않았는지
    * 결함이 일어나는 일을 막기 위해 필요한 변화를 시작한다.

### 9.6. 코드 공유

코드에 대한 책임감을 부여하기 위해 코드를 공유한다. 
주인이 없는 코드는 다른 개발자들에 의해 입맛대로 고쳐진다.
품질이 떨어지고, 팀 전체에 미칠 결과를 생각하지 않고 코드를 변경한다. 

지속적인 통합은 코드 공유를 실시하기 전에 해야하는 중요한 전제 조건이다. 
두 팀이 코드를 여러 군데 고쳐서 충돌이 발생하고, 통합하기 어려워지는 것은 낭비이다.

### 9.7. 코드와 테스트

오직 코드와 테스트만 영구 산출물로 유지한다. 
다른 문서들은 코드와 테스트에서 생성되도록 한다. 

시스템이 현재하는 일, 미래에 할 일을 만드는 것은 가치 있다. 
이 두 가지에 기여하는 산출물도 또한 가치 있다. 
나머지는 쓰레기다. 

### 9.8. 단일 코드 기반

코드 흐름은 오직 하나뿐이어야 한다. 
잠시 브랜치(branch)를 만들어 작업하는 것은 가능하지만, 몇 시간 이내로 한정시켜라. 
여러 다발의 코드 흐름은 소프트웨어 개발에서 낭비를 만든다. 

* 다른 배포된 버전들과 지금 개발이 진행 중인 브랜치에도 모두 수정이 필요하다.
* 나의 수정이 다른 브랜치에선 정상적으로 동작하지 않을 수 있다. 

코드 기반(code base)가 여러 개라면 점차 그 수를 줄여라. 
단일 코드 기반으로 작업하지 못하게 만드는 원인들을 고쳐라.

### 9.10. 매일 배치

매일 밤 새로운 소프트웨어를 제품으로 내놓아라. 
보조 실천방법인 이유는 사전에 먼저 해야하는 실천방법들이 많기 때문이다. 

* 결함 비율 낮추기
* 빌드 환경 자동화
* 배포 도구 자동화
* 배포 롤백 가능
* 팀내 신뢰도와 고객과의 신뢰도가 높은 수준으로 발달

### 9.11. 범위 협상 계약(nagotiated scope contract)

소프트웨어 개발 계약을 작성할 때 시간, 비용, 품질은 확정해도 시스템의 정확한 범위는 계속 협상해나가자고 요청한다. 
긴 계약 하나보다 짧은 계약을 여러 개 여러 번에 걸쳐 서명하여 위험도를 낮춰라. 
공급자와 고객의 이해관계를 조정한다. 
지금 보았을 때 옳아보이는 것들을 할 수 있는 용기를 준다. 

### 9.12. 사용별 지불

시스템이 사용될 때마다 돈을 청구한다. 
돈은 궁극적인 피드백 수단이다. 
릴리즈 때마다 요금을 청구하는 것은 공급자의 이기심을 부추길 수 있다. 
고객과 공급자 사이의 의사소통과 피드백을 감소시킨다. 