# MVC vs Flux

## MVC

Action -> Controller <-> Model <-> View

양방향 데이터 바인딩

모델과 뷰가 서로를 직접 업데이트 한다. - 유연성과 재사용성이 높다

확장성이 낮다. - MVC가 각각 직접 영향을 끼칠 수 있다.

## Flux

Action -> Dispatcher -> Store -> View

단방향 데이터 흐름

- 예측 가능한 상태 관리

* 장점 : 데이터 흐름의 구조화
* 단점 : 높은 학습 곡선
