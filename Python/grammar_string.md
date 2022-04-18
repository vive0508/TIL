문자열 자료형
===

## 1. 문자열 자료형
- 큰따옴표로 문자열을 만들 수 있다.
- 작은따옴표로 문자열을 만들 수 있다.
- 문자열 내부에 따옴표를 넣을 때는 하기의 방법을 이용한다.

```
print("'안녕하세요'라고 말했습니다")
print('"안녕하세요"라고 말했습니다')
print("＼"안녕하세요＼"라고 말했습니다")
print('＼'안녕하세요＼'라고 말했습니다')
```

## 2. 형변환(Cast)
- str()함수 : 매개 변수에 다른 자료형을 넣으면 값을 문자열로 변환 할 수 있다.

## 3. 문자열 연산자

| 기능 | 연산자 |
| --- | --- |
| 문자열 연결 연산자 | + |
| 문자열 반복 연산자 | \* |
| 문자 선택 연산자 | \[\] |
문자열 내부 특정 한글자를 변경하는 것은 불가능

## 4. 이스케이프 문자열

| 이스케이프 문자 | 기능 |
| --- | --- |
| ＼"  | 큰따옴표 |
| ＼'  | 작은따옴표 |
| ＼n | 줄바꿈 |
| ＼t  | 탭 |
| ＼＼ | 역슬래시 ＼ |



## 5. 문자열 관련 함수
### 5.1 `split()` 함수
문자열을 특정문자로 잘라서 리스트로 만들 때 사용

```python
print("10 20 30 40 50".split(" "))
```
['10', '20', '30', '40', '50']

### 5.2 `join()` 
함수리스트의 요소를 문자열로 연결할 때 사용
```python
print("::".join(['10','20','30','40','50'])
```
10::20::30::40::50

## ○ 레퍼런스
* [혼자 공부하는 파이썬(윤인성)](https://www.hanbit.co.kr/store/books/look.php?p_code=B2587075793)
* [이것이 취업을 위한 코딩 테스트다 with 파이썬(나동빈)](https://www.hanbit.co.kr/store/books/look.php?p_code=B8945183661)