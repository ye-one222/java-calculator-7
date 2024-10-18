# 📢 미션 설명
## ⛏ 과제 진행 요구 사항
- 미션은 문자열 덧셈 계산기 저장소를 포크하고 클론하는 것으로 시작한다.
- 기능을 구현하기 전 README.md에 구현할 기능 목록을 정리해 추가한다.
- Git의 커밋 단위는 앞 단계에서 README.md에 정리한 기능 목록 단위로 추가한다.
- AngularJS Git Commit Message Conventions을 참고해 커밋 메시지를 작성한다.
- 자세한 과제 진행 방법은 프리코스 진행 가이드 문서를 참고한다.

## ⛏ 기능 요구 사항
- 입력한 문자열에서 숫자를 추출하여 더하는 계산기를 구현한다.

- 쉼표(,) 또는 콜론(:)을 구분자로 가지는 문자열을 전달하는 경우 구분자를 기준으로 분리한 각 숫자의 합을 반환한다.
  - 예: "" => 0, "1,2" => 3, "1,2,3" => 6, "1,2:3" => 6
- 앞의 기본 구분자(쉼표, 콜론) 외에 커스텀 구분자를 지정할 수 있다. 커스텀 구분자는 문자열 앞부분의 "//"와 "\n" 사이에 위치하는 문자를 커스텀 구분자로 사용한다.
  - 예를 들어 "//;\n1;2;3"과 같이 값을 입력할 경우 커스텀 구분자는 세미콜론(;)이며, 결과 값은 6이 반환되어야 한다.
- 사용자가 잘못된 값을 입력할 경우 IllegalArgumentException을 발생시킨 후 애플리케이션은 종료되어야 한다.

## ⛏ 입출력 요구 사항
- 입력
  - 구분자와 양수로 구성된 문자열
- 출력
  - 덧셈 결과
<br/>

<hr/>


# 🎨 스스로 판단한 기능 요구 사항
- 커스텀 구분자는 문자열에서 한 번만 정의할 수 있다.
- 커스텀 구분자를 정의하면 기존의 구분자 2개와 함께 구분자로 사용된다.
<br/>

# 🧷 구현할 기능 목록
- 시작 메세지를 출력하는 메서드
- 사용자에게 문자열을 입력받는 메서드
- 문자열을 분석하는 클래스
  - 문자열을 읽고 구분자를 판단하는 메서드
  - 구분자로 문자열의 숫자를 추출하는 메서드
  - 입력 값이 잘못된 값인지 체크 (사용자가 잘못된 값을 입력할 경우 IllegalArgumentException을 발생시킴)
    - 커스텀 구분자가 한 번만 정의되는지 체크하는 메서드
    - 구분자 외 다른 문자가 등장하는지 체크하는 메서드
- 덧셈을 수행하는 클래스
- 결과 메세지를 출력하는 메서드
<br/>

<hr/>

# 🔎 구현 체크
- [ ] 시작 메세지를 출력하는 메서드
- [ ] 사용자에게 문자열을 입력받는 메서드
  - [ ] camp.nextstep.edu.missionutils에서 제공하는 Console API를 사용하여 구현해야 한다.
  - [ ] 사용자가 입력하는 값은 camp.nextstep.edu.missionutils.Console의 readLine()을 활용한다.
- [ ] 문자열을 분석하는 클래스
  - [ ] 문자열을 읽고 구분자를 판단하는 메서드
  - [ ] 구분자로 문자열의 숫자를 추출하는 메서드
  - [ ] 입력 값이 잘못된 값인지 체크 (사용자가 잘못된 값을 입력할 경우 IllegalArgumentException을 발생시킴)
    - [ ] 커스텀 구분자가 한 번만 정의되는지 체크하는 메서드
    - [ ] 구분자 외 다른 문자가 등장하는지 체크하는 메서드
- [ ] 덧셈을 수행하는 클래스
- [ ] 결과 메세지를 출력하는 메서드
