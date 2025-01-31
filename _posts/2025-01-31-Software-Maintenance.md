---
title: Software Maintenance
description: 소프트웨어개발방법및도구 강의 내용을 정리합니다.
author: Sjaize
date: 2025-01-31 22:00:00 +0800
categories: [Software Development Methodology and Tools]
tags: [git, version control]
---
# **`How multiple programmers co-work at the same time for the shared files?`**


> 혼자서 소프트웨어를 개발한다고 해도 본인이 만든 것을 일자별로
정리하기도 하고, 시험을 하기 위한 버전을 따로 관리하기도 합니다.
여러명이 같이 작업을 한다고 하면 프로그램을 어떤 식으로 유지 관리할 것인지에 대한 고민이 추가적으로 필요하겠죠. 오늘은 어떻게 서로 다른 프로그래머들이 소프트웨어의 재료가 되는 코드를 공유하고, 개발할 수 있는지 그 기술에 대해 이야기해보겠습니다.

--- 

### Version Control
![enter image description here](https://1drv.ms/i/c/6a21c25d84c6133f/IQRB2dJVmKVLSb1HT3PfTtjiAV5hya3c_Rm5oF8W90s1AHc?width=1024)
비단 소프트웨어 분야에서뿐만 아니라, **Version Control**은 아주 오래된 학문입니다. 소프트웨어가 개선이 된다고 하여 `Revision Control`, Source code를 관리하는 것이니 `Source Control` 이라고도 불리는 **Version Control**은 개선되는 버전에 대해 숫자나 글자들의 조합을 통해 변경 내용에 대한 기록을 남기는 방법입니다.

이를 통해 누군가에 의해 언제 변경이 일어났는지 기록하고 관리함으로써 문제가 생겼을 때는 그 변경 사항을 추적함으로 restored(후진) 할 수 있으며, 가지를 쳐 일부 기능에 대해서만 실험적으로 테스트를 수행하고
그 결과를 다시 merge 할 수 도 있습니다.

---
### Version Control의 형태 
1. **Centralized version control** 
![enter image description here](https://1drv.ms/i/c/6a21c25d84c6133f/IQTB31Xbdp8zT4z_G1NWZulJASt3lHQO6_3ic28zqVs-Kk0?width=1024)
가장 먼저 생각해 볼 수 있는 형태로는 중앙 집중화된 형태가 있습니다. Version Control 전용의 서버에서 소프트웨어들이 관리가 돼서 이를 통해 서로의 소프트웨어를 교환할 수 있는 형태입니다. 
	
	본인의 파일에 수정이 있을 시, 전체 내용에 바로 변화를 일으킬 수 있으므로 이것이 곧 장점이 될 수도 있고 단점이 될 수도 있습니다.

2.  **Distributed Version Control System**
![enter image description here](https://1drv.ms/i/c/6a21c25d84c6133f/IQQVHCFcMQ8BTKBZgcKrqoDTAedFBfYI7L_MufM4R0gsjnE?width=1024)
모두가 합의해 놓은 소프트웨어 버전을 다른 사람들이 다운을 받아 본인의 로컬 환경에서 수정을 가하거나, 사용자 간에 서로 변화를 동시에 주고 받거나 필요할 때에 의해서만 같은 내용을 갖도록 동기화할 수 있는 방법입니다.

> 이러한 Version Control 이론적 배경을 소프트웨어로 도구화해서 사용하는 소프트웨어를  할 수 있는 기술을 **버전 관리 시스템**이라고 부릅니다.

---
### 대표적인 버전 관리 시스템 
1. **Git**
![enter link description here](https://1drv.ms/i/c/6a21c25d84c6133f/IQQ1_gQ7TU_bSrjSLQ-ICR3sAfJ85uhM6N6NiEGi8h9qcUc?width=1024)
**Git**은 분산화된 구조를 갖고 있는 버전 처리 시스템입니다.  분산화된 구조를 갖고 있기 때문에 개별 사용자들은 개발에 필요한 모든 환경을 복사해 가지고 있기 때문에 네트워크가 끊긴 오프라인 환경에서도 개발에 문제가 없습니다. 
	
	또한, 오리지널에 대한 백업을 다 갖고 있기 때문에 중앙 집중화된 데이터베이스가 파괴되더라도 소프트웨어들이 여기저기 살아 있다는 안전성 측명이 있습니다.

3. **GitHub**
![enter image description here](https://1drv.ms/i/c/6a21c25d84c6133f/IQS78FmzWJ8NS7Hg_DEEs4MjAf0EaatDtQtNtY-kSi-iU5A?width=1024)
**GitHub**는 분산 처리 시스템인 Git의 저장소입니다. 분산 처리 시스템에 기반을 두고 있기 때문에 저장공간에 개발한 소프트웨어를 저장하고 다른 사람들이 local repository에 복사해 이용하다가 작업을 마친 후 commit, push 하는 과정을 통해 소프트웨어를 개발할 수 있습니다.

	 web 기반이기 때문에 사용하기 쉽다는 장점이 있고, bug tracking, feature request, task management 등의 부가적인 기능들을 많이 제공해서 널리 이용되는 시스템입니다.
