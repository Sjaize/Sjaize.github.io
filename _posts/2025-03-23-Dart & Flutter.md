---
title: Dart & Flutter 들어가기
description: 풀스택서비스프로그래밍-00
author: Sjaize
date: 2025-03-23 17:00:00 +0800
categories: [Dart & Flutter]
tags: [dart, flutter]
---

## **Framework**
/![(https://www.reddit.com/r/ProgrammerHumor/comments/11a1fqi/code_reuse/)](https://i.redd.it/dw23lba2qyja1.jpg)

언어만으로는 어떤 필드에 들어가서 뭔가를 개발한다는 것은 굉장히 많은 시간을 필요로 하는 일이다. 

특정한 분야에서 이미 많은 개발자들이 만들었던 것이라면 그것을 처음부터 짤 필요는 없지 않을까?

이미 만들어진 소프트웨어를 재사용해서 (Framework를 이용하여) 그 위에서 본인이 원하는 새로운 서비스를 만드는 일을 하자는 것이다.

</br>
</br>

## Flutter Framework
Framework는 특정한 언어에 의해서 만들어진다.
Django Framework는 Python, Spring Framework는 Java로 만들어졌으니, Flutter는 Dart 언어로 만들어진 Framework로 Dart와 Flutter 모두 구글에서 직접 만들었다.

</br>

#### 그렇다면 Flutter는 어떤 Framework일까?
![(https://semaphoreci.com/wp-content/uploads/2021/05/aDm0cXk.png)](https://semaphoreci.com/wp-content/uploads/2021/05/aDm0cXk.png)

화면에 뭘 표현하고 싶은 건지 (UI) 그리고 그것이 눌러졌을 때 어떤 액션이 일어날지 (User Experince)를 정의하고 그것에 맞는 버튼, 박스, 그림, 액션 코드를 찾아서 실행하는 것



</br>
</br>

## Flutter의 특징
**Cross-platform, One-source multi platform**

한 번만 그리면 된다. 안드로이드 앱으로 만든 애플리케이션을 소스코드 수정 없이 IOS, Window, Linux용으로 만들 수 있다

</br>

**Fast**

기존의 multi-platform은 virtual machine을 놓고 실행하기 때문에 native platform에 특화된 기능을 사용할 수 없었다

Flutter는 프로세서가 ARM이라면, ARM CPU에 특화된 실행 파일을 만들어주며, M 프로세서라고 하면 MacOS에 특화된 컴파일러를 통해 실행 파일을 만들어주니 빠르다.

**Productive**

앱을 개발한다고 하면 개발은 본인의 노트북이나 데스크탑에서 하고 실행은 전혀 다른 기기의 스마트폰에서 하기 때문에 노트북에서 개발한 애플리케이션을 폰으로 옮겨야 한다.

이때 테스트에서 문제가 발생했다면, 다시 컴파일 빌드를 통해 실행 파일을 뽑고 앱으로 옮겨야 하니, 케이블을 타고 디바이스로 옮기는데 시간이 소요되게 된다.

플러터는 소스 코드 레벨에서 수정을 가하면 별도의 컴파일 빌드와 앱 이동 없이 바로 디버깅 중인 디바이스에 변환되는 게 나타나니 시간을 아낄 수 있고, 이는 생산성으로 귀결된다.

**Flexible**

Flutter 내부에는 그래픽 엔진이 내장돼 있기 때문에 CPU, GPU와 직접 결합해서 그림을 그릴 수 있고, 따라서 2d 게임이나 3d 게임을 만드는 것도 가능하다

</br>
</br>

## 풀스택 서비스 프로그래머란?
![(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTw1pDoDAPDP4aKr3HjajgtEfuJBNhGo6fXdQ&s)](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTw1pDoDAPDP4aKr3HjajgtEfuJBNhGo6fXdQ&s)

통상 **클라이언트와 서버를 모두 개발할 수 있는 개발자**를 뜻한다.

하지만 회사에서 클라이언트 팀과 서버 팀이 합쳐져 있다는 것은 냉정히 말하면 이상한 일이라고 볼 수 있으니

이제는 그 의미가 달라져서 풀스택이라 말하지 않고 **서버 개발자를 뽑는데 클라이언트를 짜본 경험이 있는 자, 혹은 그 반대**, 상대방을 이해하는 자라고 말할 수 있다.