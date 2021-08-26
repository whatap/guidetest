# 에이전트 기능제어

## 에이전트 기능제어

### enabled

전체 기능을 활성화 합니다.

Java를 제외한 나머지 언어는 prefix로 whatap.를 추가해야 합니다. 예시\) whatap.enabled

{% hint style="info" %}
false인 경우에도 서버와 최소한의 통신을 유지하기 위한 정보는 전송됩니다.
{% endhint %}

```text
Default : true
Type : Boolean
```

### transaction\_enabled

트랜잭션 추적 기능을 활성화 합니다. Hitmap에 기록되는 트랜잭션 정보가 해당합니다.

```text
Default : true
Type : Boolean (enabled=false 인 경우 false)
```





whatap.name::

## Default : {type}-{ip2}-{ip3}-{port}\# +

## Type : String\# +

에이전트 이름을 패턴으로 정의 합니다.

whatap.oname::

## Default : NONE\# +

## Type : String\# +

에이전트 이름을 문자열로 정의 합니다.

whatap.okind::

## Default : NONE\# +

## Type : String\# +

에이전트가 속한 그룹 단위를 정의 합니다.

whatap.onode::

## Default : NONE\# +

## Type : String\# +

에이전트가 속한 노드 단위를 정의 합니다.

auto\_oname\_enabled::

## Default : false\# +

## Type : Boolean\# +

서버에 등록될 에이전트 이름\(oname\)을 서버로부터 자동 부여 받는 기능을 활성화 합니다. 적용 시, -Dwhatap.name, -Dwhatap.oname 옵션은 무시됩니다. 수집 서버와의 통신을 통해 oname 을 부여 받은 이후, 에이전트의 일반적인 동작을 개시합니다.

auto\_oname\_prefix::

## Default : agent\# +

## Type : String\# +

에이전트 이름을 서버로부터 자동 부여할 때 에이전트 이름의 prefix, 보통 업무 명을 사용합니다. prefix 일련번호 1~\) 부여됩니다.

auto\_oname\_reset::

## Default : 0\# +

## Type : Int\# +

서버로 부터 새로운 에이전트 이름을 부여받기 위해서 수정합니다. 에이전트 이름을 자동 부여하면 what.oname 이라는 시스템 환경 변수에 셋트됩니다. 한번 셋트되면 자바 인스턴스가 재기동 될 때까지 유지 되는데 리셋을 원할 때 auto\_oname\_reset 값을 수정합니다.\(현재 설정 값과 다른 값으로 변경하면 적용됩니다.\)

