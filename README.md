# Python-Tutorial

## PYTHON Home

```python
print("Hello, World!")
```

## PYTHON Syntax

### PYTHON 들여쓰기

####
들여쓰기는 코드 줄 시작 부분의 공백
들여쓰기를 이용해 코드 블록을 구분

```python
if 5 > 2:
  print("Five is greater than Two!")
```
❗ 들여쓰기를 건너뛰면 오류가 발생, 일반적으론 4개지만 적어도 1개는 필요 (동일한 코드 블록에서 동일한 수의 공백 사용)

ex)
```python
if 5 > 2:
  print("Five is greater than Two!")
if 10 > 5:
      print("Ten is greater than Five!!")
```

## PYTHON Comments

### 주석

####
주석은 # 으로 시작하며 PYTHON에서 무시함

```python
#This is a comment
print("Hello, World!")
```
주석은 줄 끝에도 배치 가능

```python
print("Hello, World!") # This is a comment
```
❗ 주석은 텍스트일 필요는 없음, 코드를 실행하는 것을 방지하는 데에도 사용 가능

ex)
```python
#print("Hello, World!")
print("Cheers")
```

### 여러줄 주석
PYTHON은 변수에 할당되지 않은 문자열 나열을 무시하므로 코드에 여러줄 문자열을 추가하고 주석을 넣을 수 있음

```python
"""
This is a comment
written in
more than just on line
"""
print("Hello, World!")
```

## PYTHON Variable

### 변수

####
변수는 값을 할당하면 생성됨

```python
x = 5
y = "Ji Seok KIM"
print(x)
print(y)
```
### Casting

####
데이터 유형을 지정하려면 Casting을 사용하면 됨

```python
x = str(3)    # x will be '3'
y = int(3)    # y will be 3
z = float(3)  # z will be 3.0
```

### Type()

####
함수를 이용해 변수의 데이터 유형을 알 수 있음

```python
x = 5
y = "Ji Seok KIM"
print(type(x))   # result = <class 'int'>
print(type(y))   # result = <class 'str'>
```

## PYTHON Data Types

### 데이터 유형

#### 
PYTHON엔 다양한 데이터 유형이 있음

#### 텍스트 유형 : `str`
#### 숫자 유형 : `int` `float` `complex`
#### 시퀀스 유형 : `list` `tuple` `range`
#### 매핑 유형 : `dict`
#### 세트 유형 : `set` `frozenset`
#### 부리언 유형 (참거짓을 나타내는 데 쓰임) : `bool`
#### 바이너리 유형 : `bytes` `bytearray` `memoryview`
#### 없음 유형 : `NoneType`

### 데이터 유형 설정

#### `str`  ex) x = "Hello World" 
#### `int`  ex) x = 20
#### `float` ex) x = 20.5
#### `complex` ex) x = 1j
#### `list`  ex) x = ["apple", "banana", "cherry"]
#### `tuple` ex) x = ("apple", "banana', 'cherry')
#### `range` ex) x = range(6)
#### `dict` ex) x = {"name" : "Ji Seok KIM', "age" : 20}
#### `set` ex) x = {"apple", "banana", "cherry"}
#### `frozenset` ex) x = frozenset({"apple", "banana", "cherry"})
#### `bool` ex) x = True
#### `bytes` ex) x = b"Hello"
#### `bytearray` ex) x = bytearray(5)
#### `memoryview` ex) x = memeoryview(bytes(5))
#### `NoneType` ex) x = None

## PYTHON Number

### 숫자

####
세가지 숫자 유형이 있음
- `int`
- `float`
- `complex`

```python
x = 1  #int
y = 2.8 #float
z = 1j  #complex
```
### Int

####
Int는 양수 음수 이며 소수점 이하 자릿수가 없고 길이가 무제한

```python
x = 1
y = 356462432858131
z = -32342
```

### Float

####
소수점 하나 이상을 포함하는 양수 또는 음수 숫자

```python
x = 1.10
y = 1.0
z = -35.59
```

### Complex

####
복소수는 허수 "J'를 사용

```python
x = 3+5j
y = 5j
z = -5j
```

### Random

####
PYTHON엔 랜덤함수가 없지만 모듈을 가지고 올 수 있음

```python
#1부터 9 사이의 난수를 표시함
import random #random 모듈 선언

print(random.randrange(1,10))
```

## PYTHON Strings

### 문자열

####
문자열은 ' ' 혹은 " " 으로 묶임

```python
print("Hello")
print('Hello')
```
여러 줄 문자열을 할당할 때는 """ """ 로 할 수 있음

```python
a = """ Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore mana aliqua."""
print(a)
```
### 배열

####
PYTHON의 문자열은 유니코드 문자를 나타내는 바이트 배열
[ ] 로 엑세스할 수 있음

```python
# 위치 1의 문자를 가져옴 (첫 번째 문자의 위치는 0)
a = "Hello, World!"
print(a[1]) #result = e
```
### 문자열 반복

####
for문을 사용하여 반복할 수 있음

```python
for x in "banana":
  print(x)
```
▶ 결과
```
b
a
n
a
n
a
```

### 문자열 길이

####
len()함수로 문자열 길이를 구할 수 있음

```python
a = "Hello, World!"
print(len(a)) #result = 13
```

### 문자열 확인

####
In 함수로 특정 문구나 문자가 있는지 확인할 수 있음

```python
txt = "The best things in life are free!"
print("free" in txt) #result = True
```

응용 (if문)

```python
txt = "The best things in life are free!"
if "free" in txt:
  print("Yes, "free" is present.")
```

### Slicing

####
Slice 구문으로 구문을 자를 수 있다

```python
b = "Hello, World!"
print(b[2:5])  #result = llo
```
시작 인덱스를 생략하면 범위는 첫 문자에서 시작
끝 인덱스를 생략하면 범위는 끝

```python
b = "Hello, World!"
print(b[:5])  #result = Hello
print(b[2:])  #result = llo, World!
```

### 문자열 수정

####
upper()로 문자열을 대문자로 변환 가능

```python
a = "Hello, World!"
print(a.upper())  #result = HELLO, WORLD!
```

lower()로 문자열을 소문자로 변환 가능
```python
a = "Hello, World!"
print(a.lower()) #result = hello, world!
```

strip()로 문자열에 앞 뒤 공백을 제거 가능
```python
a = "  Hello, World!   "
print(a.strip())  #result = Hello, World!
```

replace()로 문자열을 다른 문자열로 바꿀 수 있음
```python
a = "Hello, World!"
print(a.replace("H", "J") #result = Jello, World
```

split()로 문자열을 구분할 수 있음
```python
a = "Hello, World!"
print(a.split(",")) #result = ['Hello', ' World!']
```

### 문자열 연결

####
사이에 공백을 추가 하려면 " " 추가
```python
a = "Hello"
b = "World"
c = a + b
d = a + " " + b
print(c) #result = HelloWorld
print(d) #result = Hello World
```

### Format

####
format() 문자열에 숫자를 삽입 가능

```python
age = 20
txt = "My name is Ji Seok, and I am {}
print(txt.format(age)) #result = My name is Ji Seok, and I am 20
```

format()는 인수를 무제한으로 사용하며 각 자리 표시에 배치됨
{}에 숫자를 넣으면 배치할 수 있음

```python
quantity = 3
itemno = 567
price = 49.95
myorder = I want {} pieces of item {} for {} dollars."
print(myorder.format(quantity, itemno, price)) #result = I want 3 pieces of item 567 for 49.95 dollars.
```

### Escape Character

####
따옴표 안에 따옴표를 사용하면 오류가 생김
해결하기 위해 \"를 사용

```python
txt = "We are the so-called \"Vikings\" from the north." #result = We are the so-called Vikins from the north.
```

## PYTHON Operators

### 연산자

####
PYTHON 연산자는 다음 그룹으로 나눔
- 산술 연산자
- 할당 연산자
- 비교 연산자
- 논리 연산자
- 기타 연산자


### 산술 연산자

#### 더하기 `+`  ex) x + y
#### 빼기 `-`  ex) x - y
#### 곱하기 `*`  ex) x * y
#### 나누기 `/`  ex) x / y
#### 나머지 `%`  ex) x % y
#### 제곱 `**`  ex) x ** y
#### 반올림 `//`  ex) x // y

### 할당 연산자

####
#### `=` : ex) x = 5  Same As) x = 5
#### `+=` : ex) x += 3  Same As) x = x + 3
#### `-=` : ex) x -= 3  Same As) x = x - 3
#### `*=` : ex) x *= 3  Same As) x = x * 3
#### `/=` : ex) x /= 3  Same As) x = x / 3
#### `%=` : ex) x %= 3  Same As) x = x % 3
#### `//=` : ex) x //= 3 Same As) x = x // 3
#### `**=` : ex) x **= 3  Same As) x = x ** 3

### 비교 연산자

####
#### `==`  같다
#### `!=`  같지 않다
#### ` > ` 더 크다
#### ` < ` 더 작다
#### `>=` 크거나 같다
#### `<=` 작거나 같다

### 논리 연산자

####
#### `and`  둘다
#### `or`  둘중 하나
#### `not`  부정

### 기타 연산자

####
#### `is`  두 변수가 동인한 객체면 True 출력
#### `in` 변수 안에 지정된 값이 있으면 True 출력
#### `&` = `AND`
#### `|` = `OR`
#### `^` = `XOR`
#### `~` = `NOT`

## PYTHON List

### 목록 생성

####
목록은 [ ] 로 생성함
중복도 가능

```python
thislist = ['apple', 'banana', 'cherry']
print(thislist)  #result = ['apple', 'banana', 'cherry']
```

### Access

####
색인 번호로 해당 항목을 액세스 가능

```python
thislist = ['apple', 'banana', 'cherry']
print(thislist[1])  #result = ['banana']
```

시작 위치 끝 위치를 지정할 수 있음

```python
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[2:5])  #result = ['cherry', 'orange', 'kiwi']
```

시작 값을 생략가면 첫 번째 항목에서 시작됨

```python
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[:4])  #result = ['apple', 'banana', 'cherry', 'orange']
```

끝 값을 생략가면 범위가 목록 끝으로 이동함

```python
thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
print(thislist[2:])  #result = ['cherry', 'orange', 'kiwi', 'melon', 'mango']
```

In 함수로 지정된 항목이 목록에 있는지 확인 가능

```python
thislist = ["apple", "banana", "cherry"]
if "apple" in thislist:
  print("Yes, 'apple' is in the fruits list")
```

Insert 함수로 기존 값을 바꾸지 않고 새 항목을 추가 가능

```python
thislist = ["apple", "banana", "cherry"]
thislist.insert(2, "watermelon")
print(thislist)  #result = ['apple', 'banana', 'watermelon', 'cherry']
```

extend 함수로 여러개의 목록을 합칠 수 있음

```python
thislist = ["apple", "banana", "cherry"]
tropical = ["mango", "pineapple", "papaya"]
thislist.extend(tropical)
print(thislist)  #rseult = ['apple', 'banana', 'cherry', 'mango', 'pineapple', 'papaya']
```

remove 함수로 항목을 제거 가능
remove, del, pop 등등

```python
thislist = ["apple", "banana", "cherry", "banana", "kiwi"]
thislist.remove("banana")
print(thislist)  #result = ["apple", "cherry", "banana", "kiwi"]
```

clear 함수로 목록을 비울 수 있음

```python
thislist = ["apple", "banana", "cherry"]
thislist.clear()
print(thislist)   #result = []
```

### List Comprehension

####
목록의 이해는 기존 목록의 값을 기반으로 새 목록으로 생성하려는 경우 더 짧게 할 수 있음

```python
#과일 목록을 기반으로 이름에 'a'가 포함한 과일을 새 목록으로 나누는 명령문

#List Comprehension 전
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]
newlist = []

for x in fruits:
  if "a" in x:
    newlist.append(x)

print(newlist)   #result = ['apple', 'banana', 'mango']

#List Comprehension 후
fruits = ["apple", "banana", "cherry", "kiwi", "mango"]

newlist = [x for x in fruits if "a" in x]

print(newlist)   #result = ['apple', 'banana', 'mango']
```

목록을 알파벳 순으로 정렬 가능
목록을 숫자 순으로 정렬 가능 
(reverse = True) : 내림차순

```python
thislist = ["orange", "mango", "kiwi", "pineapple", "banana"]
thislist.sort()
print(thislist)  result = ['banana', 'kiwi', 'mango', 'orange', 'pineapple']
```
```python
thislist = [100, 50, 65, 82, 23]
thislist.sort()
print(thislist)  result = [23, 50, 65, 82, 100]
```

Ket = function 으로 원하는 대로 설정 할 수 있음

```python
def myfunc(n):
  return abs(n - 50)

thislist = [100, 50, 65, 82, 23]
thislist.sort(key = myfunc)
print(thislist)   #result = [50, 65, 23, 82, 100]
```

copy 기능으로 복사본 만들 수 있음
```python
thislist = ["apple", "banana", "cherry"]
mylist = thislist.copy()
print(mylist)
```

두개 이상의 목록을 결합하거나 연결 할 수 있음

- +
- append()
- extend()

## PYTHON Tuple

####
단일 변수에 여러 항목을 저장할 때 쓰임
List 와 매우 흡사
( ) 로 작성

## PYTHON Sets

####
단일 변수에 여러 항목을 저장할 때 쓰임
List 와 매우 흡사
중복된 값은 무시됨
True와 1은 동일한 값으로 처리됨
False는 0과 동일한 값으로 처리됨
{ } 로 작성

## PYTHON Dictionaries

### Dictionaries

####
Dictionaries는 쌍으로 된 데이터 값을 저장하는 데 사용됨

```python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict)  #result = {'brand': 'Ford', 'model': 'Mustang', 'year': 1964}
```

항목을 지정해서 출력 할 수 있음

```python
thisdict = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}
print(thisdict["brand"])  #result = Ford
```

이외엔 List와 흡사함

## PYTHON If..Else

### If Elif Else

####
If 로 시작해서 마지막은 Else로 끝낸다 사이는 다 Elif

```python
a = 200
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
else:
  print("a is greater than b")
```

### 짧게

####
실행문이 하나만 있는 경우 한줄에 넣을 수 있음

```python
a = 200
b = 33

if a > b: print("a is greater than b")
```

If...Else문 인 경우

```python
a = 330
b = 330
print("A") if a > b else print("=") if a == b else print("B")
```

#### `And`
#### `Or`
#### `not`

## PYTHON While Loops

### While 반복문

####
While Loop를 사용하면 조건이 참인 한 명령문을 실행할 수 있음

```python
i = 1
while i < 6:
  print(i)
  i += 1
```

### Break 문

####
```python
i = 1
while i < 6:
  print(i)
  if i == 3:
    break
  i += 1
```

### Continue 문

####
```python
i = 0
while i < 6:
  i += 1
  if i == 3:
    continue
  print(i)
```
### Else 문

####
```python
i = 1
while i < 6:
  print(i)
  i += 1
else:
  print("i is no longer less than 6")
```

## PYTHON For Loops

### Break 문

####
```python
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
  if x == "banana":
    break
```

banana일 때 루프를 종료하지만 x를 인쇄 전에 중단함

```python
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  if x == "banana":
    break
  print(x)
```

### Continue 문

####
```python
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  if x == "banana":
    continue
  print(x)
```

### Range() 문

####
```python
for x in range(6):
  print(x)
```

시작 매게변수를 사용 가능 
```python
for x in range(2, 6):
  print(x)
```

### For Else 문

####
루프가 끝나면 else문을 실행ㅏㅁㅎ

```python
for x in range(6):
  print(x)
else:
  print("Finally finished!")
```

### 중첩 루프

내부 루프는 외부 루프가 반복되 때마다 한 번씩 실행됨

```python
adj = ["red", "big", "tasty"]
fruits = ["apple", "banana", "cherry"]

for x in adj:
  for y in fruits:
    print(x, y)
```
