# 4.12 Deleting All Records from a Table

### 퀴즈

테이블에 모든 레코드를 삭제하려고합니다. 


<br>

### DELETE

아래와 같이 `DELETE` 문만 사용하여 테이블의 모든 레코드를 삭제합니다.

~~~sql
1 delete from emp
~~~

#### 주의사항

`WHERE` 절 없이 `DELETE` 명령을 수행하면 지정된 테이블에서 모든 행이 삭제됩니다. 

**동일한 명령어인 `TRUNCATE` 도 WHERE 절을 사용하지 않고 더 빠르기 때문에 DELETE보다 선호하는편입니다.** 하지만 `Oracle` 에서는 `TRUNCATE` 를 `UNDO` 할 수 없기에 주의해야합니다. 

또한 `TRUNCATE` 와 `DELETE` 간의 성능 및 롤백 방안의 차이는 각 벤더사별로 다르기 때문에 하나씩 살펴볼 필요가 있습니다.



## DELETE vs TRUNCATE 성능 차이

### Oracle



### MySQL

