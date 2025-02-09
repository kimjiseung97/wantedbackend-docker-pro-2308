## 1. 컨테이너 기술이란 무엇입니까? (100자 이내로 요약)
컨테이너는 실행에 필요한 모든 파일을 포함한 전체 실행(runtime) 환경에서 애플리케이션을 패키징하고 격리할 수 있는 기술입니다. 이를 통해 전체 기능을 유지하면서 컨테이너화된 애플리케이션을 환경(개발, 테스트, 생산 등) 간에 쉽게 이동할 수 있습니다. 컨테이너는 IT 보안의 중요한 부분이기도 합니다. 컨테이너 파이프라인에 보안을 구축하고 인프라를 보호하여 컨테이너의 안정성, 확장성, 신뢰성을 보장할 수 있습니다. 또한 일관된 행동과 기능으로 퍼블릭, 프라이빗, 하이브리드 클라우드 환경과 데이터센터(또는 온프레미스) 간에 컨테이너화된 애플리케이션을 손쉽게 이동할 수 있습니다.

## 2. 도커란 무엇입니까? (100자 이내로 요약)
도커는 컨테이너 기술을 기반으로 한 일종의 가상화 플랫폼입니다. 가상화란 물리적 자원인 하드웨어를 효율적으로 활용하기 위해서 하드웨어 공간 위에 가상의 머신을 만드는 기술이고, 컨테이너란 컨테이너가 실행되고 있는 호스트 os의 기능을 그대로 사용하면서 프로세스를 격리해 독립된 환경을 만드는 기술을 뜻합니다.

## 3. 도커 파일, 도커 이미지, 도커 컨테이너의 개념은 무엇이고, 서로 어떤 관계입니까?
Application을 포장 및 전송하기 위해 도커는 "docker image"를 사용한다.

Docker image는 파일로 어플리케이션 실행에 필요한 독립적인 환경을 포함하며, 런타임 환경을 위한 일종의 템플릿이다.


도커 이미지는 소스 코드, 라이브러리, 종속성, 도구 및 응용 프로그램을 실행하는데 필요한 기타 파일을 포함하는 불변(변경 불가) 파일이다.

이미지는 읽기 전용이므로 스냅샷이라고도 하며, 특정 시점의 애플리케이션과 가상 환경을 나타낸다.

이러한 일관성은 도커의 큰 특징 중 하나로 개발자가 안정적이고 균일한 조건에서 소프트웨어를 테스트하고 실험할 수 있도록 한다.


도커 컨테이너란?

사용자가 기본 시스템에서 애플리케이션을 분리할 수 있는 가상화된 런타임 환경이다.

이러한 컨테이너는 응용프로그램을 빠르고 쉽게 시작할 수 있는 portable units 이다.

중요 기능은 컨테이너 내부에서 실행되는 컴퓨팅 환경의 표준화다. (standardization of the computing environment running inside the container.)

응용 프로그램이 동일한 환경에서 작동하도록 할 뿐 아니라 다른 사람과의 공유도 단순화한다.


컨테이너는 자율적(autonomous)이기 때문에 strong isolation을 제공하며 서로 방해하지 않는다. -> 격리

하드웨어 수준에서 가상화가 이루어지는 VM과 달리 컨테이너는 애플리케이션 계층에서 가상화된다.

하나의 머신을 활용하고 커널을 공유하며 분리된 프로세스를 실행하기 위한 운영 체제를 가상화할 수 있다.

따라서 컨테이너가 매우 가벼워져 리소스를 많이 사용하지 않을 수 있다.