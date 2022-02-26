# 클래스
## 클래스 사용 방법
### 초기화
```
class 클래스명 {
	//클래스 scope
}
``` 
> 변수(property)와 함수(method)의 모음

클래스를 메인에서 초기화시켜 사용한다.
메인에서 초기화 시키면 클래스가 인스턴스화 된다.
인스턴스 = 메모리에 로드되어 있는 클래스


클래스 = 인스턴스를 만드는 틀 (붕어빵 틀)
인스턴스 = 클래스를 이용해서 만들어 내는 서로 다른 속성의 객체를 지칭하는 용어 (그 틀로 찍어내는 붕어빵들 ex. 슈크림 붕어빵, 팥 붕어빵, 딸기 붕어빵 etc)

### companion object
``` 
companion object{
	//매소드와 프로퍼티
}
``` 
> 초기화 없이 사용 가능하다.

## 클래스 생성자
생성자 : constructor
- 인스턴스의 속성을 초기화
- 인스턴스 생성시 구문을 수행

보조 생성자
constructor(필요한 생성자)


# 상속
## 상속을 사용하는 이유
1. 기존 작성된 코드를 재활용하기 위함
2. 코드 재활용하는데 > 체계적인 구조로 사용하기 위해서

```
open class Parent{
	// open을 앞에 써서 상속 가능한 클래스로 만들어준다.
    
    var money = 50
    var house = "20평 아파트"
    
    
   open fun showHouse(){
    //재정의 가능한 함수로 만들기 위해 open을 붙여준다.
    }
}

class Child : Parent() {
	// : 쓰고 상속 받는 클래스를 써주고, ()를 써서 초기화 한다.
    
    //상속받은 Parent 클래스의 프로퍼티와 매서드를 내것처럼 사용할 수 있다.
	
    override fun showHouse(){
    //부모 클래스에 있는 동일한 함수 이름을 재정의 하기위해 override를 붙여준다.
    //상속 관계에서만 사용, 재정의 하기 위해
    }
}
```


## 오버로드
```
class Son {

	fun getNum( Z:string ) : Int{
    	return 1
    }
    
    fun getNum( Z:string, H:String) : Int{
    	return 2
    }
}
```

> 동일한 이름이지만 파라미터의 구성이 다른 함수를 만드는 것
