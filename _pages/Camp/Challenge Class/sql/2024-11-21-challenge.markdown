---
title: Day1
date: 2024-10-30 21:00:00
categories: [캠프, 챌린지반]
tags:
  [
    캠프
  ]
---

https://school.programmers.co.kr/learn/courses/30/lessons/59407

SELECT ANIMAL_ID FROM ANIMAL_INS WHERE NAME IS NOT NULL;

https://school.programmers.co.kr/learn/courses/30/lessons/59035

SELECT NAME, DATETIME FROM ANIMAL_INS ORDER BY ANIMAL_ID DESC;


https://school.programmers.co.kr/learn/courses/30/lessons/59408

SELECT SUM(CNT) AS CNT FROM (
SELECT COUNT(DISTINCT(NAME)) AS CNT FROM ANIMAL_INS
WHERE NAME IS NOT NULL
) A;

SELECT SUM(NAME) COUNT FROM (
SELECT COUNT(DISTINCT(NAME)) AS NAME FROM ANIMAL_INS
WHERE NAME IS NOT NULL
GROUP BY NAME
) A  GROUP BY NAME;