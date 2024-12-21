---
title: Day1
date: 2024-10-30 21:00:00
categories: [캠프, 챌린지반]
tags:
  [
    캠프
  ]
---

데이터 그룹화

1. GROUP BY 
    ```sql
    SELECT ITEM, SUM(COST) FROM MENU
    GROUP BY ITEM
    ```

2. 

정렬

1. ORDER BY 
  ```sql
  SELECT ITEM, SUM(COST) FROM MENU
  GROUP BY ITEM
  ORDER BY DESC -- 내림차순
  ```

HAVING 그룹화된 결과에 조건을 걸 때 사용

```sql
SELECT item, SUM(sales) FROM Cafe
GROUP BY 
HAVING SUM(sales) >= 10000
ORDER BY sales DESC;

SELECT item , COUNT(*) FROM Cafe
GROUP BY item
HAVING COUNT(*) >= 2
ORDER BY count DESC;

```