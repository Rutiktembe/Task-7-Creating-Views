# Task-7-Creating-Views
HERE ARE MY RELATIONAL TABLES
SQL> select *
    from emp;

     EMPNO ENAME      JOB              MGR HIREDATE         SAL       COMM     DEPTNO
---------- ---------- --------- ---------- --------- ---------- ---------- ----------
      7369 SMITH      CLERK           7902 17-DEC-80        800                    20
      7499 ALLEN      SALESMAN        7698 20-FEB-81       1600        300         30
      7521 WARD       SALESMAN        7698 22-FEB-81       1250        500         30
      7566 JONES      MANAGER         7839 02-APR-81       2975                    20
      7654 MARTIN     SALESMAN        7698 28-SEP-81       1250       1400         30
      7698 BLAKE      MANAGER         7839 01-MAY-81       2850                    30
      7782 CLARK      MANAGER         7839 09-JUN-81       2450                    10
      7788 SCOTT      ANALYST         7566 19-APR-87       3000                    20
      7839 KING       PRESIDENT            17-NOV-81       5000                    10
      7844 TURNER     SALESMAN        7698 08-SEP-81       1500          0         30
      7876 ADAMS      CLERK           7788 23-MAY-87       1100                    20
      7900 JAMES      CLERK           7698 03-DEC-81        950                    30
      7902 FORD       ANALYST         7566 03-DEC-81       3000                    20
      7934 MILLER     CLERK           7782 23-JAN-82       1300                    10



  SQL> SELECT *
   FROM DEPT;

    DEPTNO DNAME          LOC
---------- -------------- -------------
        10 ACCOUNTING     NEW YORK
        20 RESEARCH       DALLAS
        30 SALES          CHICAGO
        40 OPERATIONS     BOSTON


      
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


      
