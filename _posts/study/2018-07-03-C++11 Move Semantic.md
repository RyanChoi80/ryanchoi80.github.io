---
layout: post
comments: true
categories: study
---

* 유용한 링크 : http://itguru.tistory.com/189
* 이동의미론( move semantic )
  * C++11에서 추가된 개념. 객체의 복사시에 불필요한 객체의 생성, 소멸을 막기 위해 생겨난 개념...? 
  * 참조를 왼값참조(&), 오른값참조(&&)로 구분.
     * 왼값 : 메모리 공간을 할당받고 주소를 가지고 있어서 &연산자로 접근 가능.
     * 오른값 : 왼값이 아닌 값.
   * 오른값참조변수는 왼값이다. std::move로 오른값으로 바꿔줘서 사용한다.
   * std::move : 왼값, 오른값을 받아 오른값으로 변환해준다.
  * 전달참조(forwarding reference) : 형식연역( & + && = & )에 따라 왼값이나 오른값이 될수 있다.
  * std::forward : 전달참조(forwarding reference)에 사용. 왼값, 오른값을 받아 왼값이나, 오른값으로 변환해준다.
