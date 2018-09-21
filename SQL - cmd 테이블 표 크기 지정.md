# CMD 창에서 oracle DB 실행시키기.
```
경로 > sqlplus
Enter user-name: 
Enter password :
SQL> 
```


# CMD 창에서 MySQL 실행시키기
```
~ > cd mysql\bin 파일 경로
mysql\bin 파일 경로 > mysql -uroot -p
Enter password:*******

mysql > show database
mysql > use 사용할 database
mysql > show table
```
![cmd mysql 실행 error](https://user-images.githubusercontent.com/42515875/45861081-bba1d980-bda5-11e8-9e54-647d4aff13f6.png)
# CMD 창에서 MySQL 못 불러오는 오류 - ```ERROR 2003 (HY000): Can't connect to MySQL server on 'localhost' (10061)```

> 제어판 -> 시스템 보안 -> 관리도구 -> 서비스 -> mysql 찾아서 서비스 **시작**
![cmd mysql 실행 error 해결](https://user-images.githubusercontent.com/42515875/45861087-c0ff2400-bda5-11e8-95fc-4fe42f0447fc.png)
# CMD 창에서 ORACLE DB로 테이블 select해올 때 크기 조절

```
SQL> SET PAGESIZE 200
SQL> SET LINESIZE 140

```

