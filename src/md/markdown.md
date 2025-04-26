# 마크다운 문법

* [마크다운이란?](#마크다운이란?)
* [베이직 마크다운 문법](#베이직-마크다운-문법)
  1. [Headings](#1-headings)
  2. [Paragraphs](#2-paragraphs)
  3. [Line Breaks](#3-line-breaks)
  4. [Emphasis](#4-emphasis)
  5. [Blockquotes](#5-blockquotes)
  6. [Lists](#6-lists)
  7. [Code Blocks](#7-code-blocks)
  8. [Horizontal Rules](#8-horizontal-rules)
  9. [Links](#9-links)
  10. [Images](#10-images)
  11. [Escaping Characters](#11-escaping-characters)
  12. [Tables](#12-tables)
  13. [Task Lists](#13-task-lists)

---

## 마크다운이란?
마크다운은 일반 텍스트 문서에 서식 요소를 추가할 때 쓸 수 있는 마크업 랭귀지이다. 2004년에 John Gruber에 의해 만들어졌고, 지금 세계에서 가장 인기있는 마크업 랭귀지 중 하나이다.

---

## 베이직 마크다운 문법

### 1. Headings
헤딩을 사용하기 위해서는 해쉬 사인(#)을 글자 앞에 붙이면 된다. 한개부터 여섯개까지 사용 가능. 제대로 출력하기 위해서는 마크업 문법 적용된 라인 위, 아랫줄에 빈 줄을 넣어야 한다.

###### 예시&출력

`##### Heading level 5`

##### Heading level 5


`#### Heading level 4` 

#### Heading level 4

또는 헤딩 레벨 1 또는 2 사용 시 글자 밑 줄에 여러개의 =(헤딩 레벨 1) 또는 -(헤딩 레벨 2)를 추가하면 똑같은 효과를 줄 수 있다.

###### 예시&출력

```markdown
헤딩 레벨 2
---------------
```

헤딩 레벨 2
---------------

### 2. Paragraphs
새 단락을 추가할 때 빈 줄을 사용해 단락을 분리할 수 있음.

### 3. Line Breaks
줄을 나누고 싶을때는 두개 이상의 스페이스를 넣고 엔터를 칩니다.  
하지만 스페이스는 있는지 없는지 확인하기가 어려우니, 마크다운 앱에서 HTML을 서포트 한다면 `<br>` 태그를 사용해도 좋다.

### 4. Emphasis
글자를 강조하고 싶을 때, 두꺼운 글자(Bold) 또는 기운 글자(Italic)를 사용할 수 있음.

#### Bold

별표(*) 또는 언더바(_)를 강조하고 싶은 글자 앞뒤에 2개씩 넣어서 사용 가능.
한 단어 안의 글자를 강조하고 싶을때는 띄어쓰기 없이 추가하면 똑같이 적용 가능.

###### 예시&출력

`공부를 **열심히** 하자` → 공부를 **열심히** 하자  
`공부를 __열심히__ 하자` → 공부를 __열심히__ 하자  
`멋쟁이**사자**처럼` → 멋쟁이**사자**처럼  

#### Italic  

별표(*) 또는 언더바(_)를 강조하고 싶은 글자 앞뒤에 1개씩 넣어서 사용 가능.
한 단어 안의 글자를 강조하고 싶을때는 띄어쓰기 없이 추가하면 똑같이 적용 가능.

###### 예시&출력

`공부를 *열심히* 하자` → 공부를 *열심히* 하자  
`공부를 _열심히_ 하자` → 공부를 _열심히_ 하자  
`멋쟁이_사자_처럼` → 멋쟁이_사자_처럼  

#### Bold and Italic  

Bold and Italic 두가지 한꺼번에 적용하고 싶은 경우 별표(*) 또는 언더바(_)를 강조하고 싶은 글자 앞뒤에 3개씩 넣어서 사용 가능.
한 단어 안의 글자를 강조하고 싶을때는 띄어쓰기 없이 추가하면 똑같이 적용 가능.

###### 예시&출력

`공부를 ***열심히*** 하자` → 공부를 ***열심히*** 하자  
`공부를 ___열심히___ 하자` → 공부를 ___열심히___ 하자  
`멋쟁이***사자***처럼` → 멋쟁이***사자***처럼  

### 5. Blockquotes  

상자안에 인용을 넣고 싶다면 오른쪽 화살표 기호(>)를 문장 앞에 넣어주면 된다.

###### 예시&출력

`> 공부를 열심히 하자`

> 공부를 열심히 하자

#### Blockquotes with Multiple Paragraphs  

상자안에 여러개의 단락을 넣고 싶다면 오른쪽 화살표 기호(>)를 빈 줄에 넣으면 된다.

###### 예시&출력

```markdown
> 공부를 열심히 하자
>
> 할 수 있다!
```

> 공부를 열심히 하자
>
> 할 수 있다!

#### Nested Blockquotes

상자안에 상자를 또 만들고 싶다면, 안에 넣고싶은 단락 앞에 오른쪽 화살표 기호(>)를 2개 넣으면 된다.

###### 예시&출력

```markdown
> 공부를 열심히 하자
>
> > 할 수 있다!
```

> 공부를 열심히 하자
>
> > 할 수 있다!

#### Blockquotes with Other Elements

상자안에 다른 요소를 넣어 만들 때. 오른쪽 화살표 기호(>)를 다른 요소로 적용할 단락 앞에 넣으면 된다.
주의! 모든 요소가 적용되는 것은 아니다.

###### 예시&출력

```markdown
> 공부를 열심히 하자
>
> > #### 오늘의 학습
> >
> > - CLI 명령어 연습하기
> > - 마크다운 문법 연습하기
>
> 화이팅!
```

> 공부를 열심히 하자
>
> > ##### 오늘의 학습
> >
> > - CLI 명령어 연습하기
> > - 마크다운 문법 연습하기
>
> 화이팅!

### 6. Lists
리스트를 만들어 정리할 수 있다.

#### Ordered Lists

숫자를 넣어 리스트 만들기. 리스트하고 싶은 글자 앞에 숫자와 마침표를 넣으면 됨. 처음 리스트 아이템은 1로 시작해야하고, 나머지 숫자는 순서대로 넣을 필요 없음.
리스트의 리스트를 만들고 싶을때는 숫자 앞에 스페이스(공백)을 4개 넣어주면 됨.

###### 예시&출력

```markdown
**일반 리스트**
1. 첫번째 아이템
2. 두번째 아이템
3. 세번째 아이템  

**리스트의 리스트**
1. 첫번째 아이템
    1. 첫번째 아이템의 첫번째 아이템
    1. 첫번째 아이템의 두번째 아이템
1. 두번째 아이템
1. 세번째 아이템
```

**일반 리스트**
1. 첫번째 아이템
2. 두번째 아이템
3. 세번째 아이템  

**리스트의 리스트**
1. 첫번째 아이템
    1. 첫번째 아이템의 첫번째 아이템
    1. 첫번째 아이템의 두번째 아이템
1. 두번째 아이템
1. 세번째 아이템

#### Unordered List

순서 없는 리스트를 만들때는 대쉬(-), 별표(*) 또는 플러스(+) 사인을 각 아이템 앞에 넣어주면 된다.

###### 예시&출력

```markdown
* 첫번째 아이템
* 두번째 아이템
    * 두번째 아이템의 첫번째 아이템
    * 두번째 아이템의 두번째 아이템
* 세번째 아이템
```

* 첫번째 아이템
* 두번째 아이템
    * 두번째 아이템의 첫번째 아이템
    * 두번째 아이템의 두번째 아이템
* 세번째 아이템

#### Starting Unordered List Items With Numbers

순서 없는 리스트 아이템의 글자가 숫자로 시작하고 그 숫자가 마침표로 끝나는 경우에는, 백래쉬(\)를 숫자와 마침표 사이에 넣으면 됨.
예시의 두번째 줄은 백래쉬를 안했을 경우 원하던 대로 출력되지 않는 것을 확인할 수 있음.

###### 예시&출력

```markdown
- 2004\. 이천사년
- 2004. 이천사년
```

- 2004\. 이천사년
- 2004. 이천사년

#### Adding Elements in Lists

리스트 안에 요소를 넣고 싶은 경우에는 글자 앞에 공백 4개를 넣거나 tab을 한 번 넣어주면 된다.

###### 예시&출력

```markdown
* 첫번째 아이템
* 두번째 아이템
    두번째 아이템은 책상 위에 있음.
* 세번째 아이템
```

* 첫번째 아이템
* 두번째 아이템
    두번째 아이템은 책상 위에 있음.
* 세번째 아이템

### 7. Code Blocks
글에 코드 블럭을 넣고 싶은 경우에는 백틱(`)을 사용. 코드 시작과 끝 부분에 백틱 3개를 붙인다. 시작 부분 백틱에 사용 프로그래밍 언어를 명시할 수 있음.

###### 예시&출력

````markdown
```javascript
console.log('Hello');
```
````

```javascript
console.log('Hello');
```

#### Code

글 중간에 코드로 된 글자를 만들고 싶다면 백틱(`)을 글자 앞뒤에 추가.

###### 예시&출력

```markdown
터미널에 `code .`을 입력하세요.
```

터미널에 `code .`을 입력하세요.


### 8. Horizontal Rules
구분선을 넣고싶다면 별표(*), 대쉬(-) 또는 언더바(_)를 3개 이상 넣으세요.

###### 예시&출력

```markdown
***
-----
```

***
-----

### 9. Links
링크를 넣고싶다면 대괄호([])안에 글자를 넣고 그 뒤에 소괄호(())를 이용하여 링크를 입력하세요.

###### 예시&출력

```markdown
제 [깃헙 페이지](https://github.com/chajiiiii)를 방문해보세요!
```

제 [깃헙 페이지](https://github.com/chajiiiii)를 방문해보세요!

#### Adding Titles on Links
링크에 마우스를 올리면(hover) 보이는 타이틀을 추가할 수 있다. 위의 링크 추가 방법에서 URL 다음에 쌍따옴표("")를 이용하여 타이틀을 입력.

###### 예시&출력

```markdown
제 [깃헙 페이지](https://github.com/chajiiiii "최고")를 방문해보세요!
```

제 [깃헙 페이지](https://github.com/chajiiiii "최고")를 방문해보세요!

#### URLs and Email Addresses
URL와 이메일 주소를 링크로 만들고 싶다면 화살표 괄호(<>)안에 URL과 이메일 주소를 넣으세요.

###### 예시&출력

```markdown
<https://github.com/chajiiiii>
```

<https://github.com/chajiiiii>


### 10. Images
이미지를 넣으려면 줄 앞에 느낌표(!)를 넣고, 뒤에 대괄호([])를 이용하여 안에 대체 텍스트를 넣고, 뒤에 소괄호(())를 이용하여 이미지 URL 또는 path를 입력합니다.

예시

```markdown
![지현 뒷모습](../assets/me.jpg "최고")
```

![지현 뒷모습](../assets/me.jpg "최고")

#### Linking Images
이미지를 클릭하면 링크로 이동하는 방법. 위의 이미지 입력 방식을 대괄호([])로 감싼 후 이미지 대괄호 뒤에 소괄호(())로 링크 입력.

###### 예시&출력

```markdown
[![지현 뒷모습](../assets/me.jpg "최고")](https://www.google.com/search?gs_ssp=eJzj4tDP1TfISLYwMWD0Ys9LLS8sTawEADSUBdE&q=newquay&oq=newqu&gs_lcrp=EgZjaHJvbWUqBwgBEC4YgAQyBggAEEUYOTIHCAEQLhiABDINCAIQLhivARjHARiABDIHCAMQABiABDIHCAQQABiABDIHCAUQABiABDIHCAYQABiABDINCAcQLhivARjHARiABDIHCAgQLhiABNIBCDQ1NjdqMGo3qAIAsAIA&sourceid=chrome&ie=UTF-8)
```

[![지현 뒷모습](../assets/me.jpg "최고")](https://www.google.com/search?gs_ssp=eJzj4tDP1TfISLYwMWD0Ys9LLS8sTawEADSUBdE&q=newquay&oq=newqu&gs_lcrp=EgZjaHJvbWUqBwgBEC4YgAQyBggAEEUYOTIHCAEQLhiABDINCAIQLhivARjHARiABDIHCAMQABiABDIHCAQQABiABDIHCAUQABiABDIHCAYQABiABDINCAcQLhivARjHARiABDIHCAgQLhiABNIBCDQ1NjdqMGo3qAIAsAIA&sourceid=chrome&ie=UTF-8)


### 11. Escaping Characters
특수기호를 문자로 쓰고 싶을경우에는 백래쉬(\)를 기호 앞에 써주면 됩니다.

###### 예시&출력

```markdown
\*기호 앞에 백래쉬를 붙이세요.
```

\*기호 앞에 백래쉬를 붙이세요.

### 12. Tables
표를 만들고 싶다면 3개 이상의 대쉬(-)를 사용하여 헤더를 구분하고, 파이프(|)를 이용하여 컬럼을 구분하세요. 대쉬 갯수는 3개 이상이면 동일하지 않아도 가능.

###### 예시&출력

```markdown
|색상|영어|
|---|----|
|빨강|Red|
|노랑|Yellow|
```

|색상|영어|
|---|----|
|빨강|Red|
|노랑|Yellow|


### 13. Task Lists
체크 리스트를 만들 때는 대쉬(-) 뒤에 공백이 사이에 있는 대괄호([ ])를 붙여 리스트 아이템을 작성합니다. 체크 된 상태로 표시하고 싶을때는 대괄호([])안에 x 를 작성합니다.

###### 예시&출력

```markdown
- [x] 1주차 숙제 완료
- [ ] 2주차 숙제 완료
```

- [x] 1주차 숙제 완료
- [ ] 2주차 숙제 완료

* [맨 위로 가기](#마크다운-문법)