---
title: Anomalous States of Knowledges as a Basis for Information Retrieval
draft: false
tags:
---

안없어지자나...
Nicholas J. Belkin

그동안의 information retrieval 연구 -> System의 속성(document representation, channel같은거)에 포커스
IR을 cognitive 관점-> 특히
이 연구는 user's anomalous state of Knowledge라는 관점에서 보고자 함

IR 시스템 디자인에 있는 문제에 대한 해결책이 됨

IR은 problem-oriented discipline
- transfer of desired information between human generator <-> human user
- 인간들간의 직접적인 의사소통, 환경으로 부터 직접 지식을 얻는 것은 포함안됨
이 논문에서 information=a particular structure associated with a text
텍스트전체.(그 부분이 아니라)
focus on whole texts or combinations of texts
텍스트란? semiotic structure. 문서를 포괄하는 개념

IR시스템의 역할: 사람들이 문제를 해결하도록 도와주는것,(not solving the problems themselves)

IR situation:
1. 정보요구를 recognize한 유저가 request
2. IR은 들어온 request에 기반해서 사용자의 정보요구를 만족시킬 것 같은 text를 present
3. user의 평가. 정보요구가 만족되었는가? 부분적으로?완전히?아예노노?->usefulness/relevance of the text to the need

IR communication system

저자(generator, author): 커뮤니케이션하자!, her state of Knowledge (<-modified by beliefs, intention, values, ...) (<-linguistic, pragmatic rules to become the text)
독자(user): 내 지식의 상태를 점검해보자!->불완전하군 -> recognized anomalous state of knowledge(ask)
이제 request를 시스템에 넣는데 이것또한 modified by linguistic, pragmatic...

이러한 communication의 성공여부는 얼마나 독자의 anaomaly가 해결되었는가에 달려있음 -> ==독자(정보의 recipient==에 달려있고, iterative함)

독자의 역할 강조
-> representation에 있어서 corpus of need가 저장된 corpus of document(text representation)만큼 중요하다

appropriate rules for need representation
(왜냐고? 봐, IR system을 평가할때 유저의 knowledge상태에 달려있자나, 저자가 아니라)
appropriate rules for need representation를 먼저 고려하고 그 틀 안에서 적절한 text representation 과 retrieval strategies를 고려해야 함

ASK에 대하여
- taylor의 정보질문의 4단계중 앞의 두단계
	- internal -> conscious(realized)
- kochen의 problems, needs, requests간의 관계 중 앞에 두개
- wersig: individual's recognition of a problematic situation
gaps, lacks, uncertainty, incohernece..등등의 wrongness,
-> 이 문제를 해결하기 위해서 information이 필요하다

즉 공통적으로 무엇을 모르는지 모르는 상태
-> 이 저자는 anomalous라는 용어 제안
non-specifiability의 문제도 설명할수 있음
when IR system is evaluated, difference between relevance as predicted by the system and relevance as assigned by the human <- 왜? <-request가 그 request기저에 딸려있는 요구와는 잘 맞지 않아서

0쪽: a problem is recognized, it is also recognized that information might be necessary to resolve the problem, but because of the inquirer's lack of knowledge about the problem area, it is impossible to specify what would resolve it

##### Implications of ASKs for IR
따라서 "best match"는 적절한 원칙이 아니다(이건 well specified anomalies에서만 적절함)
such systems depend crucially upon exact specification

documents representation보다 ASKs representations을 먼저 개발해야겠지

다양한 종류의 ASKs에 따라 다양한 retrieval strategies가 필요

그러다면 user's knowledge of the problem을 발견하고 표현하는 수단을 강구해야 함 
- ex)avoid placing mechanism-related constraints upon the user,
- ex) through dialouge, rather than specification

이런 IR system은 당연히 iterative interaction이어야 하고 성능에 대한 평가도 이에 기반해서 이루어져야 함
->in terms of how well the mechanism has interpreted and represented the user's ASK, and whether an appropriate retrieval strategy was chosen