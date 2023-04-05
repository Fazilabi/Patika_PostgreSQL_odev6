# Patika_PostgreSQL_odev6

## [Patika.dev](www.patika.dev)

### 1. film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?
`SELECT AVG(rental_rate) FROM film;`

### 2. film tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar?
`SELECT COUNT(*) FROM film` <br>
`WHERE title ILIKE 'c%';`

### 3. film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?
`SELECT rental_rate, length FROM film` <br>
`WHERE rental_rate = '0.99'` <br>
`ORDER BY length DESC` <br>
`LIMIT 1 ;`

### 4. film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?
`SELECT COUNT(DISTINCT replacement_cost)  FROM film`<br>
`WHERE length > 150 ;`
