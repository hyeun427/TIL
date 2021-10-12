# [210912 animation]

## 1. animation

- 애니메이션 효과를 줄 수 있다.

## 2. @keyframes

- @ 규칙은 개발자가 애니메이션 중간 중간의 특정 지점들을 @keyframes를 통해 설정한다.

- 사용법
> @keyframes 프레임명 { </br>
>   from { 스타일 작성 }</br>
>   to { 스타일 작성 }</br>
> }
> </br>
> or</br>
>  @keyframes 프레임명 { </br>
>   0% { 스타일 작성 }</br>
>   50% { 스타일 작성 }</br>
>   100% { 스타일 작성 }</br>
> }

## 3. animation-name, animation-duration

- animation-name
  - 애니메이션 이름을 지정한다.

- animation-duration
  - 애니메이션이 한 사이클을 완료하는데 걸리는 시간을 지정한다.
  - s, ms를 단위로 쓰며, 음수값은 사용이 불가하다.

## 4. animation-delay, animation-timing-function

- animation-delay
  - 애니메이션이 언제 시작할지 설정한다.
  - s, ms를 단위로 쓰며 음수값도 가능하다.
  - 음수의 경우(-n), 애니메이션이 n초부터 재생된다.

- animation-timing-function
  - 애니메이션 진행 속도를 지정한다.
  - linear | ease | ease-in | ease-out | ease-in-out | step-start | step-end | steps(int,start|end) | cubic-bezier(n,n,n,n) 중 하나를 선택할 수 있다.

## 5. animation-iteration-count, animation-direction

- animation-iteration-count
  - 애니메이션의 재생(반복) 횟수를 설정한다.
  - 정수 값을 넣으면 된다.
  - infinite는 무한히 반복하는 것을 의미한다.

- animation-direction
  - 애니메이션의 재생 방향을 설정한다.
    - normal: 정방향 재생
	- reverse: 역방향 재생
	- alternate: 정방향과 역방향으로 한 번씩 번갈아 재생(정방향 시작)
    - alternate-reverse: 역방향과 정방향으로 한 번씩 번갈아 재생(역방향 시작)

## 6. animation-play-state

- 애니메이션의 처음 실행 상태를 결정한다.
- paused: 애니메이션이 일시 중지된 상태를 유지함.
- running: 애니메이션이 재생중인 상태임. 디폴트.

## 7. animation-fill-mode

- 애니메이션 실행 전과 후의 스타일을 지정한다.
- none: 디폴트. 애니메이션 중이 아닌 경우, 요소의 CSS 스타일을 유지함.
- forwards: 애니메이션 중이 아닌 경우, 애니메이션 마지막 키프레임의 CSS 스타일을 유지 함.
- backwards: 애니메이션 중이 아닌 경우, 첫 번째 애니메이션 키프레임의 CSS 스타일을 유지 함.(지연 시간 포함)
- both: 애니메이션 시작 전에는 첫 번째 애니메이션 키프레임을 유지하며, 종료 후에는 마지막 키프레임 애니메이션의 CSS 스타일을 유지함. "none" 과는 다름.
- "none" 과 "backwards" 속성 값은 애니메이션 중이 아닌 경우 다른 화면을 표시할 수 있으므로 주의해야 함.

## 8. 단축속성

- ```animation : 이름 지속시간 속도 지연시간 반복횟수 연결방향;```

- 시간 값이 duration과 delay 두개이므로 duration, delay 순서대로 작성한다.