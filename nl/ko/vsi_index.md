---



copyright:
  years: 2017, 2018
lastupdated: "2018-10-05"


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}
{:pre: .pre}
{:tip: .tip}
{:table: .aria-labeledby="caption"}

# 시작하기 튜토리얼
{{site.data.keyword.BluVirtServers}}는 수 분 내에 배치할 수 있습니다. 가상 서버는 사용자의 워크로드에 적합한 지역에 사용자가 선택한 가상 서버 이미지로부터 배치됩니다.
{:shortdesc}

가상 프라이빗 클라우드에서 IBM Virtual Server를 사용해 보십시오! 자세한 정보는 [IBM Cloud Virtual Servers for VPC](../../docs/vsi-is/getting-started.html#gettingstartedvsigen)를 참조하십시오.
{:tip}

가상 서버 작성 시에는 공용(멀티 테넌시) 환경 또는 전용(싱글 테넌시) 환경 중에서 선택할 수 있습니다. 그런 다음, 선택한 환경에 따라 시간별, 월별 또는 임시 가상 서버도 선택해야 합니다. 공용 가상 서버의 경우, SAN 기반 스토리지 또는 로컬 스토리지가 사용되도록 선택합니다.

## 시작하기 전에

시작하기 전에 다음 전제조건을 검토하십시오.

  1. 가상 서버를 주문하려면 업그레이드된 계정이 있어야 합니다. 이 프로세스는 어느 정도 시간이 소요될 수 있으며 계속하려면 사용자의 요청이 승인되어야 합니다. 계정 업그레이드에 대한 자세한 정보는 [IBM ID로 전환](https://console.bluemix.net/docs/admin/softlayerlink.html)을 참조하십시오.
  2. 배치 옵션을 검토하고 선택하십시오. 자세한 정보는 다음 주제를 참조하십시오.

|배치 옵션                           |설명                                        |
| --------------------------------------------------------- | --------------------------------------------------- |
|[공용 가상 서버](../vsi/vsi_public.html)            |IBM 관리 멀티 테넌시 가상 서버 배치|
|[임시 가상 서버](../vsi/vsi_about_transient.html)|감소된 비용으로 유연성 있는 워크로그에 최적화되어 제공되는 IBM 관리 멀티 테넌시 가상 서버 배치 |
|[예약된 가상 서버](../vsi/vsi_about_reserved.html)  | 계약 기간 동안 용량이 보장되는 IBM 관리 멀티 테넌시 가상 서버 배치 |
|[전용 가상 서버](../vsi/vsi_dedicated.html)      |IBM 관리 싱글 테넌시 가상 서버 배치            |
{: caption="표 1. 배치 옵션" caption-side="top"}   

## 가상 서버 프로비저닝

배치 옵션을 결정한 후에는 프로비저닝 프로세스를 시작하십시오.

|프로비저닝 지시사항                                         |설명                                            |
| -------------------------------------------------------------------------- | ------------------------------------------------------- |
|[공용 인스턴스 프로비저닝](../vsi/vsi_provision_public.html)                |다양한 옵션으로 공용 인스턴스를 프로비저닝             |
|[임시 인스턴스 프로비저닝](../vsi/vsi_provision_transient.html)                |다양한 옵션으로 임시 인스턴스 프로비저닝            |
|[예약된 용량 및 인스턴스 프로비저닝](../vsi/vsi_provision_reserved.html)            | 다양한 옵션으로 예약된 용량 및 인스턴스 프로비저닝 |
|[전용 호스트 및 인스턴스 프로비저닝](../vsi/vsi_provision_dedicated.html)|개인용 인스턴스 또는 전용 인스턴스를 전용 호스트에 프로비저닝함|
{: caption="표 2. 프로비저닝 정보" caption-side="top"}

## 다음 단계

가상 서버가 프로비저닝되어 사용 가능한 상태가 되면 {{site.data.keyword.slportal_full}} 또는 {{site.data.keyword.slapi_full}}를 사용하여
가상 서버를 구성할 수 있습니다. 자세한 정보는 [가상 서버 구성](../vsi/vsi_configuring.html)을 참조하십시오.
