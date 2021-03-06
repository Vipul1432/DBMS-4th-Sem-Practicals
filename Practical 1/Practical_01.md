# P1 : To study DDL-create and DML-insert commands

## Create tables according to the following definition

<hr>

CREATE TABLE DEPOSIT (ACTNO VARCHAR2(5) ,CNAME VARCHAR2(18) ,
BNAME VARCHAR2(18) , AMOUNT NUMBER(8,2) ,ADATE DATE);

CREATE TABLE BRANCH(BNAME VARCHAR2(18),CITY VARCHAR2(18));

CREATE TABLECUSTOMERS(CNAME VARCHAR2(19) ,CITY VARCHAR2(18));
CREATE TABLE BORROW(LOANNO VARCHAR2(5), CNAME VARCHAR2(18),
BNAME VARCHAR2(18), AMOUNT NUMBER (8,2));
<hr>

![image](https://user-images.githubusercontent.com/81670997/174234967-bd8bcd51-382c-4d59-9310-e8ef71eabc08.png)

![image](https://user-images.githubusercontent.com/81670997/174235053-55b44a04-c007-4fb1-ab82-c3399defa89e.png)

![image](https://user-images.githubusercontent.com/81670997/174235142-7e308569-26e4-495b-b878-23ae24eefaf3.png)

![image](https://user-images.githubusercontent.com/81670997/174235270-c29f4870-a5f8-4938-aa63-32f37c36fde0.png)

<hr>

# DEPOSIT

INSERT INTO DEPOSIT VALUES('100',’ANIL’,'VRCE',1000,'1-MAR-95');<br>
INSERT INTO DEPOSIT VALUES('101','SUNIL','AJNI',5000,'4-JAN-96');<br>
INSERT INTO DEPOSIT VALUES('102','MEHUL','KAROLBAGH',3500,'17-NOV-95');<br>
INSERT INTO DEPOSIT VALUES('104','MADHURI','CHANDI',1200,'17-DEC-95');<br>
INSERT INTO DEPOSITVALUES('105','PRMOD','M.G.ROAD',3000,'27-MAR-96');<br>
INSERT INTO DEPOSIT VALUES('106','SANDIP','ANDHERI',2000,'31-MAR-96');<br>
INSERT INTO DEPOSIT VALUES('107','SHIVANI','VIRAR',1000,'5-SEP-95');<br>
INSERT INTO DEPOSIT VALUES('108','KRANTI','NEHRUPLACE',5000,'2-JUL-95');<br>
INSERT INTO DEPOSIT VALUES('109','MINU','POWAI',7000,'10-AUG-95');<br>

<hr>

# BRANCH

INSERT INTO BRANCH VALUES('VRCE','NAGPUR');<br>
INSERT INTO BRANCH VALUES('AJNI','NAGPUR');<br>
INSERT INTO BRANCH VALUES('KAROLBAGH','DELHI');<br>
INSERT INTO BRANCH VALUES('CHANDI','DELHI');<br>
INSERT INTO BRANCH VALUES('DHARAMPETH','NAGPUR');<br>
INSERT INTO BRANCH VALUES('M.G.ROAD','BANGLORE');<br>
INSERT INTO BRANCH VALUES('ANDHERI','BOMBAY');<br>
INSERT INTO BRANCH VALUES('VIHAR','BOMBAY');<br>
INSERT INTO BRANCH VALUES('NEHRU PLACE','DELHI');<br>
INSERT INTO BRANCH VALUES('POWAI','BOMBAY');<br>

<hr>

# CUSTOMER

INSERT INTO CUSTOMERS VALUES ('ANIL','CALCUTTA');<br>
INSERT INTO CUSTOMERS VALUES ('SUNIL','DELHI');<br>
INSERT INTO CUSTOMERS VALUES ('MEHUL','BARODA');<br>
INSERT INTO CUSTOMERS VALUES ('MANDAR','PATNA');<br>
INSERT INTO CUSTOMERS VALUES ('MADHURI','NAGPUR');<br>
INSERT INTO CUSTOMERS VALUES ('PRAMOD','NAGPUR');<br>
INSERT INTO CUSTOMERS VALUES ('SANDIP','SURAT');<br>
INSERT INTO CUSTOMERS VALUES ('SHIVANI','BOMBAY');<br>
INSERT INTO CUSTOMERS VALUES ('KRANTI','BOMBAY');<br>
INSERT INTO CUSTOMERS VALUES ('NAREN','BOMBAY');<br>

<hr>

# BORROW

INSERT INTO CUSTOMERS VALUES ('ANIL','CALCUTTA');<br>
INSERT INTO CUSTOMERS VALUES ('SUNIL','DELHI');<br>
INSERT INTO CUSTOMERS VALUES ('MEHUL','BARODA');<br>
INSERT INTO CUSTOMERS VALUES ('MANDAR','PATNA');<br>
INSERT INTO CUSTOMERS VALUES ('MADHURI','NAGPUR');<br>
INSERT INTO CUSTOMERS VALUES ('PRAMOD','NAGPUR');<br>
INSERT INTO CUSTOMERS VALUES ('SANDIP','SURAT');<br>
INSERT INTO CUSTOMERS VALUES ('SHIVANI','BOMBAY');<br>
INSERT INTO CUSTOMERS VALUES ('KRANTI','BOMBAY');<br>
INSERT INTO CUSTOMERS VALUES ('NAREN','BOMBAY');<br>

<hr>

## From the above given tables perform the following queries

<hr>

<b>1. Describe deposit, branch.</b>

DESC DEPOSIT;

![image](https://user-images.githubusercontent.com/81670997/174236105-5b417e69-81d7-4651-a559-0971b462095e.png)

<hr>

DESC BRANCH;

![image](https://user-images.githubusercontent.com/81670997/174236220-610b897a-9b65-4fc5-98f6-3ffc2f48f6d6.png)
<hr>

<b>2. Describe borrow, customers.</b>

DESC BORROW;

![image](https://user-images.githubusercontent.com/81670997/174236610-eaa73270-4d89-4190-bcb0-d3e3b0e8ac52.png)

<hr>

DESC CUSTOMERS;

![image](https://user-images.githubusercontent.com/81670997/174236772-f4036306-c6e7-4ccc-a521-2635273116e1.png)

<hr>

<b>3. List all data from table DEPOSIT.</b>

SELECT * FROM DEPOSIT;

![image](https://user-images.githubusercontent.com/81670997/174239687-e55b55c0-0fe5-49d5-a482-1f59b5b62739.png)

<hr>

<b>4. List all data from table BORROW.</b>

SELECT * FROM BORROW;

![image](https://user-images.githubusercontent.com/81670997/174239915-ee937390-8659-4865-8e7c-b0c869c7d8d5.png)

<hr>

<b>5. List all data from table CUSTOMERS.</b>

SELECT * FROM CUSTOMERS;

![image](https://user-images.githubusercontent.com/81670997/174240126-34cd66e8-163c-4a66-9f0d-f3dd78ef2ba9.png)

<hr>

<b>6. List all data from table BRANCH.</b>

SELECT * FROM BRANCH;

![image](https://user-images.githubusercontent.com/81670997/174240330-87def592-27a2-4090-983b-7b1763360bc3.png)

<hr>

<b>7. Give account no and amount of depositors.</b>

SELECT ACT NO,AMOUNT FROM DEPOSIT;

![image](https://user-images.githubusercontent.com/81670997/174240531-aca37d2e-8948-4e8f-8dd2-322b87123c3e.png)

<hr>

<b>8. Give name of depositors having amount greater than 4000.</b>

SELECT CNAME FROM DEPOSITE WHERE AMOUNT >4000;

![image](https://user-images.githubusercontent.com/81670997/174240759-76731687-2f49-4e91-801a-397bf3934f45.png)

<hr>

<b>9. Give name of customers who opened account after date '1-12-96'.</b>

SELECT C_NAME FROM DEPOSITE WHERE DATE > ‘1-DEC-96’;

![image](https://user-images.githubusercontent.com/81670997/174241090-5a891358-9740-400f-91c5-9f048545f837.png)

<hr>
