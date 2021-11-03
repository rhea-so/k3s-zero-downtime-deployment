# 왜 무중단 배포가 필요할까요?

모든 것이 빠르게 변하는 시대입니다. 그중에서도 IT, 특히 소프트웨어 분야의 역동성은 남다릅니다.   
최근 들어 많은 개발자들이 체감하는 가장 큰 변화로 배포(Deployment) 빈도의 증가를 꼽을 수 있습니다.   
소프트웨어 개발 방법론이 폭포수(Waterfall) 방식에서 애자일(Agile) 방식으로 바뀌면서 릴리즈 주기가 긴 소프트웨어는 줄어들었습니다.  
그만큼 제품은 더 빨리 출시되며 기능 추가와 보완을 위해 더 자주 배포되고 있습니다.

서비스는 과거 하나의 거대한 아키텍처로 구현되는 모놀리식(Monolithic) 구조에서 마이크로서비스(Microservices)로 모듈화되어 독립적으로 개발하고 동시에 배포할 수 있게 되었습니다.  
잦은 배포는 시장과 고객의 비즈니스 요구를 빠르게 충족시키고 서비스의 가치를 높입니다.  
하지만 운영 안정성 측면에서는 부정적인 영향을 미칠 수 있습니다.  
그렇기 때문에 배포는 **위험을 최소화하고 안정적으로 수행해야 합니다.**

## 무중단 배포란?

무중단 배포는 서비스 장애와 배포의 부담을 최소화하기 위해 운영 중인 서비스를 중단하지 않고,  
신규 소프트웨어를 배포하는 기술입니다.

무중단 배포의 핵심은 로드 밸런서를 통해 연결된 두 개 이상의 인스턴스에 트래픽을 제어해 배포하는 것입니다.

배포 작업이 서비스에 영향을 주지 않도록 하기 위해 고객의 이용량에 따라 인스턴스는 물론,  
로드밸런서도 다중화를 고려해야 합니다.  

즉, 무중단 배포를 하기 위해서는 고가용성의 시스템 인프라가 구성되어 있어야 합니다.

## 이제 한번 알아봅시다!

* [무중단 배포를 안 할 경우](./02_ReCreate.md)
* [롤링 배포](./03_RollingUpdate.md)
* [블루 그린 배포](./04_BlueGreenRelease.md)
* [카나리 배포](./05_CanaryRelease.md)