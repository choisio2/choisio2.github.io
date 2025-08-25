---
title: "Kotlin 기본 문법 정리"
description: >-
    Kotlin 기본 문법 
    타입, 형변환, 문자열, 함수
date: 2025-08-25 00:10
author: sio2
categories: [Android Studio, Kotlin]
tags: [Kotlin]
---


# Kotlin 문법
------------
## 변수 선언
```
val x = 10   // 선언시에만 초기화 -> 변경 불가능 
var y = 20   // 변경 가능
```


------------
## 타입 & 형변환
* Int, Double, Boolean, String 
* null 허용 -> 타입 뒤에 '?' 더해주기 -> 없으면 null값 불가능 
```
var name: String? = null
val x: Int = 10
val y: Double = x.toDouble()
val str = x.toString()
val num = "123".toInt()
```


------------
## 문자열 
```
val name = "Sujung"
println("My name is $name and length is ${name.length}")
```


------------
## 조건문 
```
val x = 3
if(x > y) {
	println(x)
} else{
	println(y)
}

when(x){
	1 -> println("One")
	in 2..5 -> println("2 to 5")
	else -> println("Other")
}  
```


------------
## 반복문
```
for(i in 1..5) println(i)   // 1~5
for(i in 5 downTo 1 step 2) println(i)   // 5, 3, 1

while(x > 0) {x--}   
```
------------
## 함수 
```
fun main(){ 
	println(add(1, 2))
}
fun add(a: Int, b: Int): Int{
	return a+b;
} 

```
------------
## 배열
```
val arr = arrayOf(1, 2, 3)
println(arr[0])      // 1
arr[1] = 10          // 값 변경

val arr2 = intArrayOf(1, 2, 3) // 기본 타입 배열
```
------------
## 문자열 & 인덱스 
```
val s = "Hello"
println(s[0])        // H
for (ch in s) print(ch)  // H e l l o
```
------------
## 리스트 
```
val list = listOf("a", "b", "c")        // 불변
val mList = mutableListOf("a", "b")     // 가변
mList.add("c")
println(mList[0])  // a
```


