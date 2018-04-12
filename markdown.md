마크다운 markdown 문법
======================

# 1. Headers
## 1.1. 큰제목: 문서 제목
	```
	This is an H1
	=============
	```
	This is an H1
	=============

## 1.2. 작은제목: 문서 부제목
	```
	This is an H2
	-------------
	```
	This is an H2
	-------------

## 1.3. 글머리: 1~6까지만 지원
	```
	# This is a H1
	## This is a H2
	### This is a H3
	#### This is a H4
	##### This is a H5
	###### This is a H6
	```

# 2. BlockQuote
블럭인용문자(```>```))를 이용한다.
```
> This is a blockqute.
```
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.

이 안에서는 다른 마크다운 요소를 포함할 수 있다.
> ### This is a H3
> * List
>	```
>	code
>	```

# 3. 목록
## 3.1. 순서있는 목록(번호)
순서있는 목록은 숫자와 점을 사용한다.
```
1. 첫번째
2. 두번째
3. 세번째
```
1. 첫번째
2. 두번째
3. 세번째

순서는 내림차순으로 정의된다.
```
1. 첫번째
3. 세번째
2. 두번째
```
1. 첫번째
3. 세번째
2. 두번째

## 3.2. 순서없는 목록(글머리 기호)
```
* 빨강
	* 녹색
		* 파랑

+ 빨강
	+ 녹색
		+ 파랑

- 빨강
	- 녹색
		- 파랑
```
* 빨강
	* 녹색
		* 파랑

+ 빨강
	+ 녹색
		+ 파랑

- 빨강
	- 녹색
		- 파랑

## 3.3. 혼합해서 사용이 가능하다.
```
* 1단계
	- 2단계
		+ 3단계
			= 4단계
```

* 1단계
	- 2단계
		+ 3단계
			= 4단계

# 4. 코드```<pre><code></code></pre>```
4개의 공백 또는 하나의 탭으로 들여쓰기를 만나면 변환되기 시작하여, 들여쓰지 않은 행을 만날때까지 변환이 계속된다.

> 한줄 띄어쓰면 인식이 제대로 안되는 문제가 발생하하기도 한다.

```
This is a normal paragraph:

    This is a code block.
end code block.
```

<code>
```
This is a normal paragraph:
    This is a code block.
end code block.
```
</code>

실제로 적용해보면,
This is a normal paragraph:

    This is a code block.
end code block.

# 5. 수평선```<hr/>```
수평선을 만든다. 마크다운 문서를 미리보기로 출력할 때 *페이지 나누기* 용도로 많이 사용한다.
```
* * *

***

*****

- - -

---------------------------------------
```

* * *

***

*****

- - -

---------------------------------------


# 6. 링크
## 6.1. 참조링크

```
[link keyword][id]
[id]: URL "Optional Title here"

Link: [Google][googlelink]
[googlelink]: https://google.com "Go google"
```

Link: [Google][googlelink]
[googlelink]: https://google.com "Go google"

## 6.2. 인라인 링크
```
syntax: [Title](link)
```

Link: [Google](https://google.com, "google link")

## 6.3. 자동연결
```
<http://example.com/>
<address@example.com>
```

<http://example.com/>
<address@example.com>

#7. 강조
```
*single asterisks*
_single underscores_
**double asterisks**
__double underscores__
++underline++
~~cancelline~~
```
*single asterisks*
_single underscores_
**double asterisks**
__double underscores__
++underline++
~~cancelline~~

## 8. 이미지
```
![Alt text](/path/to/img.jpg)
![Alt text](/path/to/img.jpg "Optional title")
```
![박보영 프로필 사진](https://search.pstatic.net/common?type=a&size=120x150&quality=95&direct=true&src=http%3A%2F%2Fsstatic.naver.net%2Fpeople%2Fportrait%2F201312%2F20131211170041770-2535427.jpg)
![박보영 프로필 사진](https://search.pstatic.net/common?type=a&size=120x150&quality=95&direct=true&src=http%3A%2F%2Fsstatic.naver.net%2Fpeople%2Fportrait%2F201312%2F20131211170041770-2535427.jpg "박보영 프로필 사진")

사이즈 수정 시 ```<img width="" height=""></img>```를 이용한다.

****