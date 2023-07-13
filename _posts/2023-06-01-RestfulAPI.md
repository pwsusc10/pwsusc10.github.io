---
layout: post
title: RESTful APIfks?
subtitle: Rest? REST API의 특징?
categories: TIL
tags: [Rest API]
---

## REST란?

REST => Representational State Transfer (대표하는 상태를 전송)  
Software Architecture 중 하나. / Network-based Software Architectures

## RESTful API

두 컴퓨터 시스템이 인터넷을 통해 정보를 안전하게 교환하기 위해 사용하는 인터페이스.

## REST Architecture style의 6 principles

1. Statelessness => 요청들은 독립적이어야 한다.(http protocol)
2. Cacheability => (http protocol)
3. Layered System
4. Code on demand
5. Uniform interface!! => 가장 중요!
   - Resource Identification in requests
   - Resource manipulation through representations
   - Self-descriptive messages
   - Hypermedia as the engine of application state(HATEOAS)

## RESTful API의 장점

1. Scalability => 클라이언트와 서버 사이의 상호 작용을 최적화하기 때문에 효율적으로 크기를 조정할 수 있다.
2. Flexibility => 클라이언트와 서버의 완전한 분리를 할 수 있다. 각 부분이 독립적으로 개발될 수 있도록 다양한 서버 구성 요소를 단순화하고 분리한다.
3. Independence => REST API는 사용되는 기술과 독립적이다. API 설계에 영향을 주지 않고 다양한 프로그래밍 언어로 클라이언트 및 서버 애플리케이션을 모두 작성할 수 있다. 또한 통신에 영향을 주지 않고 양쪽의 technology를 변경할 수 있다.
