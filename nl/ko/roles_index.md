---

copyright:
  years: 2016, 2018
lastupdated: "2018-02-23"

---

{:new_window: target="blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}

# 사용자, 애플리케이션 및 게이트웨이 역할

역할은 특정 오퍼레이션에 대한 액세스를 부여하거나 제한하기 위해 사용할 수 있는 권한 세트입니다. 역할을 사용하여 사용자, 애플리케이션 및 게이트웨이 그룹에 대한 권한을 관리할 수 있습니다.
{:shortdesc}

## 사용자 역할
{: #user_roles}

{{site.data.keyword.iot_full}}에 사용자를 추가, 초대 또는 등록할 때 사용자 역할을 지정할 수 있습니다. {{site.data.keyword.iot_short_notm}} 대시보드를 사용하여 언제든 사용자 역할을 지정하거나 변경할 수도 있습니다. 사용자에게 역할을 지정하는 데 대한 자세한 정보는 [사용자 역할 관리](managing_user_roles.html)를 참조하십시오.

사용할 수 있는 표준 사용자 역할은 다음과 같습니다.

사용자 역할 |설명
------------- | -------------
관리자 |모든 사용자 관련 API에 액세스를 부여하는 '수퍼유저' 역할입니다. 관리자는 디바이스와 애플리케이션으로 제한되는 오퍼레이션에 액세스할 수 없습니다.
오퍼레이터 |프론트 엔드 조직 사용자용입니다. 대부분의 조직 오퍼레이션, 액세스 제어 오퍼레이션, 써드파티 오퍼레이션 및 위험 관리 오퍼레이션에 대한 액세스를 부여합니다.

개발자 |디바이스 오퍼레이션, 로그 오퍼레이션, 캐시 오퍼레이션, 히스토리언 오퍼레이션 및 써드파티 서비스 오퍼레이션에 대한 무제한 액세스를 부여합니다. 이 역할은 조직, 액세스 제어 및 위험 관리 오퍼레이션에 제한된 액세스를 제공합니다.
독자 |기본 사용자 역할입니다. 모든 사용자가 사용할 수 있는 오퍼레이션에 대해 제한된 액세스를 부여합니다.

사용자 역할에 대한 자세한 정보는 [사용자 역할](reference/roles_access.html)을 참조하십시오.

## 애플리케이션 역할
{: #application_roles}
특정 오퍼레이션에 대한 애플리케이션 액세스를 부여하거나 거부하는 애플리케이션 역할을 지정할 수 있습니다. 모든 애플리케이션 역할은 다음 오퍼레이션에 대한 액세스를 거부합니다.

- 모든 위험 관리 오퍼레이션
- 스토리지 매개변수 구성
- 인증 제공업체 구성
- 이메일 구성 작성, 업데이트 또는 삭제

사용할 수 있는 표준 애플리케이션 역할은 다음과 같습니다.

애플리케이션 역할 |설명
------------- | -------------
표준 |기본 애플리케이션 역할입니다. 사용자나 역할 오퍼레이션을 제외한 대부분의 애플리케이션 오퍼레이션에 대한 액세스를 부여합니다.   
오퍼레이션 |가장 광범위한 오퍼레이션에 대한 액세스를 부여하지만 구독 또는 공개 오퍼레이션에 대한 액세스는 거부합니다.
백엔드 신뢰 |시스템 연산자가 상호작용하지 않아도 되는 애플리케이션용입니다. 디바이스 관리, 조직, 역할 또는 확장기능 오퍼레이션에 대한 액세스를 거부합니다.
데이터 프로세서 |분석과 데이터 처리를 수행하는 애플리케이션용입니다. 데이터 프로세서 애플리케이션에는 조직 오퍼레이션과 사용자 오퍼레이션에 대한 제한된 액세스가 부여됩니다. 
시각화 |데이터의 시각화 생성을 담당하는 애플리케이션용입니다. 시각화 애플리케이션은 라이브 및 저장된 데이터 오퍼레이션과 대시보드 오퍼레이션에 액세스합니다.
디바이스 |디바이스 역할을 수행하는 애플리케이션용입니다. 즉, 디바이스인 것처럼 {{site.data.keyword.iot_short_notm}}에 전송되는 데이터 소스를 제공합니다. 디바이스 애플리케이션에는 오퍼레이션에 대한 제한된 액세스만 부여됩니다.

애플리케이션 역할의 오퍼레이션 액세스에 대한 자세한 정보는 [애플리케이션 역할](reference/app_roles_access.html)을 참조하십시오.

## 게이트웨이 역할
{: #gateway_roles}
게이트웨이에는 {{site.data.keyword.iot_short_notm}}에 디바이스를 등록하는 기능과 게이트웨이 정의를 제어하는 제한된 수의 역할이 있습니다.

사용할 수 있는 표준 게이트웨이 역할은 다음과 같습니다.

게이트웨이 역할 |설명
------------- | -------------
표준 |오퍼레이션에 대한 제한된 액세스를 부여합니다. 표준 게이트웨이는 게이트웨이 지정 리소스 그룹 내에 있는 디바이스 대신 작동하도록 제한됩니다.
권한이 부여됨 |기본 게이트웨이 역할입니다. 신뢰된 게이트웨이용이며 권한 부여된 게이트웨이가 {{site.data.keyword.iot_short_notm}}에 디바이스를 추가하도록 허용합니다. 디바이스 및 디바이스 특성을 추가, 업데이트 및 관리하는 데 적합한 오퍼레이션에 대한 액세스를 부여하지만 다른 오퍼레이션에 대한 액세스 권한은 없습니다.  

게이트웨이 역할의 오퍼레이션 액세스에 대한 자세한 정보는 [게이트웨이 역할](reference/gateway_roles_access.html)을 참조하십시오.
