## 변수 선언
**var** 변경 가능
**val** 변경 불가 > 런타임시 변경 안 하는 변수

클래스에 선언 : Property (속석)
이외 Scope 에 선언 : 로컬 변수

변수에 값 할당 안 될 경우 에러
자료형 뒤에 ?붙이면 nullable 변수로 사용 가능

(초기화를 늦추는 lateinit, lazy 등도 존재)

## 기본 자료형
- 정수형 / 실수형
- Char
- Boolean : true or false


## 조건문
```
if (조건문) {
	} else { 
    }
```

## for문
```
for (index in 1..10) {
	Log.d (TAG, "${index}입니다.")
    Log.d (TAG, "$index")
    }
```

> 로그창에 index라는 변수가 1부터 10까지 반복 출력

```
for (index in 1..10) {
	textLog.append ("${index}")
    }
```

> textLog라는 tv에 텍스트가 1~10까지 추가되어 출력 (여러줄)

