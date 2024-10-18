# 문자열 덧셈 계산기
***
## 요구 기능
+ 빈 문자열 ("") 입력시 0을 반환
+ 쉼표(,), 콜론(:)을 구분자로 가지는 문자열을 전달하는 경우 구분자를 기준으로 분리한 각 숫자의 합을 반환
+ 커스텀 구분자 생성
    + //와 \n사이에 위치한 문자를 커스텀 구분자로 사용할 수 있음
+ 잘못된 값을 입력하면 "[ERROR]"로 시작하는 에러 메시지를 출력한 후 프로그램 종료

***
## 기능 명세

+ 입력값 관리
    + 빈 문자열 입력 관리
        + input이 비어있으면 0 출력
    + 커스텀 구분자 관리
        + 문자열이 //로 시작 할 경우 \n전까지 변수로 저장
        + \n까지 잘라내고 남은 문자열의 합을 출력
        + 오류
            + 커스텀 문자열이 하나 이상일 경우
    + 에러처리
        + 구분자로 나누었을 때 number가 아니면 error
        + 커스텀 구분자 이외 숫자가 아닌 다른 문자가 있으면 error
        + 입력값에 음수가 있으면 error
        + ,,,,,2 처럼 구분자 사이에 공백이 있을경우

+ 프로그램 종료
    + process.exit()를 호출하지 않고 종료