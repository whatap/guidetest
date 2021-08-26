# 에이전트 공통 옵션

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

