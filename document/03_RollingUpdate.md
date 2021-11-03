# 하나씩 새걸로 바꿔켜기

minReadySeconds : pod이 Ready 단계 부터 Available 단계 까지 식단 차이 시간을 설정하지 않으면 ready에서 곧바로 avaliable이 되고 순단 현상이 일어난다. 적절한 시간을 테스트하여 설정하는것이 좋다.

strategy.type : “Recreate” or “RollingUpdate”를 설정가능. 기본값은 “RollingUpdate”, Recreate의 경우 Pod가 삭제된 후 재생성

strategy.rollingUpdate.maxSurge : rolling update 중 정해진 Pod 수 이상으로 만들 수 있는 Pod의 최대 개수. 기본값은 25%

strategy.rollingUpdate.maxUnavailable : rolling update 중 unavailable 상태인 Pod의 최대 개수를 설정. rollgin update 중 사용할 수 없는 Pod의 최대 개수. 값은 0보다 큰 정수를 통해 Pod의 절대 개수 설정이 가능하고, “25%“와 같이 percentage 표현 가능 . maxUnavailable에서 percentage 계산은 rounding down(내림) 방식이며 기본값은 25% 이다. maxSurge와 maxUnavailable 값이 동시에 0이 될 수 없다.

19번 이미지까지 업로드하면 됨.
