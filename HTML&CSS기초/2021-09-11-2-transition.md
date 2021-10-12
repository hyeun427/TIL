# [210911 transition]

## 1. transition

- transition 속성은 정해진 시간 동안 요소의 속성값을 부드럽게 변화시킨다.
- 시간의 개념이 들어간다!
- 속성
  - transition-property : 요소에 추가할 transition 효과를 설정한다.
  - transition-duration : transition 효과가 지속될 시간을 설정한다.
  - transition-delay : transition 효과가 나타나기 전까지의 지연 시간을 설정한다.
  - transition-timing-function : transition 효과의 시간당 속도를 설정한다.
    - ease : 빠르게-느리게
    - linear : 일정하게
    - ease-in : 느리게-빠르게
    - ease-out : 빠르게-느리게
    - ease-in-out : 느리게-빠르게-느리게

## 2. 단축속성

- ```transition: property duration timing-function delay; ```
- 숫자를 적으면 앞 숫자는 duration, 뒤 숫자는 delay에 해당된다.