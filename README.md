# sqlEleventhTask
## Bu repo [Patika.dev](https://www.patika.dev) tarafından verilen `SQL` ödevini içermektedir.
---
### Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.
### 1- actor ve customer tablolarında bulunan first_name sütunları için tüm verileri sıralayalım.
- (
-	SELECT first_name FROM actor
-	ORDER BY first_name ASC
- )
- UNION
- (
-	SELECT first_name FROM customer
-	ORDER BY first_name ASC
- );
### 2- actor ve customer tablolarında bulunan first_name sütunları için kesişen verileri sıralayalım.
- (
-	SELECT first_name FROM actor
-	ORDER BY first_name ASC
- )
- INTERSECT
- (
-	SELECT first_name FROM customer
-	ORDER BY first_name ASC
- );
### 3- actor ve customer tablolarında bulunan first_name sütunları için ilk tabloda bulunan ancak ikinci tabloda bulunmayan verileri sıralayalım.
- (
-	SELECT first_name FROM actor
-	ORDER BY first_name ASC
- )
- EXCEPT
- (
-	SELECT first_name FROM customer
-	ORDER BY first_name ASC
- );
### 4- İlk 3 sorguyu tekrar eden veriler için de yapalım.
- İlk sorgu için UNION ALL
- İkinci sorgu için INTERSECT ALL
- Üçüncü sorgu için EXCEPT ALL
