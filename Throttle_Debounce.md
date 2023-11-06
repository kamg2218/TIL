# Throttle vs Debounce

## Throttle

특정 시간에 한 번 목록을 업데이트하는 것을 의미한다.
입력이 시작되면, **일정 주기로 계속 실행한다.**

```jsx
timeoutID = setTimeout(debounceMode ? clear : exec, delay);
```


## Debounce

사용자가 타이핑을 멈출 때까지 기다렸다가 목록을 업데이트하는 것을 의미한다.
마지막 이벤트에서 일정 시간 동안 이벤트가 발생하면, 또 일정 시간을 기다린다.
입력이 끝날때까지 무한적으로 기다린다.

```jsx
export default function (delay, callback, options) {
	const { atBegin = false } = options || {};
	return throttle(delay, callback, { debounceMode: atBegin !== false });
}
```

## 참고 자료

[throttle-debounce](https://github.com/niksy/throttle-debounce)
