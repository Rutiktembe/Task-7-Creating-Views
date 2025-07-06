# Task-7-Creating-Views


1.Use CREATE VIEW with complex SELECT



SQL> SELECT
  2      E.EMPNO,
  3      E.ENAME AS EmployeeName,
  4      D.DNAME AS Department,
  5      E.SAL
  6  FROM EMP E
  7  JOIN DEPT D ON E.DEPTNO = D.DEPTNO;

     EMPNO EMPLOYEENA DEPARTMENT            SAL
---------- ---------- -------------- ----------
      7369 SMITH      RESEARCH              800
      7499 ALLEN      SALES                1600
      7521 WARD       SALES                1250
      7566 JONES      RESEARCH             2975
      7654 MARTIN     SALES                1250
      7698 BLAKE      SALES                2850
      7782 CLARK      ACCOUNTING           2450
      7788 SCOTT      RESEARCH             3000
      7839 KING       ACCOUNTING           5000
      7844 TURNER     SALES                1500
      7876 ADAMS      RESEARCH             1100
      7900 JAMES      SALES                 950
      7902 FORD       RESEARCH             3000
      7934 MILLER     ACCOUNTING           1300


      
