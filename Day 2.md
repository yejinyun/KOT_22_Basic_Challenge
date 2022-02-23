# 형변환과 배열
## 형변환
- 명시적 형변환
to~~()
Kotlin에 해당

- 암시적 형변환
변수 할당시, 자료형 지정 안 해도 자동으로 형 변환

## 배열
```
var intArr = arrayOf(1,2,3,4,5)
```
> 배열 변수 선언, arrayOf 함수로 배열 저장 값 나열

```
var nullArr = arrayOfNulls<Int>(5)
```
> null로 채워진 길이 5의 배열, 자료형은 Int

```
var intArr[2] = 8
```
> 해당 인덱스에 값 할당
