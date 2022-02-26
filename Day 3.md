# 타입 추론
- 변수, 함수 선언시, 연산 시에 코틀린이 자동으로 자료형을 추론해주는 기능
	-> 코드량을 줄여준다.
- 코틀린의 특징  

# 함수

## fun
- 기본 함수
```
fun 함수이름() {
	//코드 블럭 (scope)
    }
```

- 입력값이 있는 함수
```
fun functionParam(param : String) {

	}
```

- 출력값이 있는 함수
```
fun getPi() : Double(타입명시) {
	return 3.14
	}
```

- 예시
```
fun add(a:Int, b:Int, c:Int) : Int(){
	return a+b+c
    }
```

a,b,c 는 모두 Int형,
함수의 반환값도 Int형

- 단일 표현식 함수
```
fun add(a:Int, b:Int, c:Int) = a+b+c
```
위의 '예시'와 같은 함수
반환형의 타입추론이 가능 > 반환형 안 써도 됨

## override fun
부모 클래스에 메서드를 재정의 하기 위해서는
1. 부모 클래스의 메서드에 open 키워드 달기
2. 자식 클래스 메서드에 override 키워드달기

> 부모 클래스의 함수를 override 하는 함수의 경우 항상 붙여줘야함.


[참고]

[강의 1](https://youtu.be/9f7rBip7xc0)
[강의 2](https://youtube.com/playlist?list=PLQdnHjXZyYadiw5aV3p6DwUdXV2bZuhlN)
[override fun](https://greedy0110.tistory.com/68)
