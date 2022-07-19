# sql6
patika.dev linkim: https://app.patika.dev/cmilakonur <br />

1- film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir? <br />
SELECT ROUND(AVG(rental_rate),2) FROM film; <br />

2- film tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar? <br />
SELECT COUNT(*) FROM film <br />
WHERE title LIKE 'C%'; <br />

3- film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır? <br />
SELECT MAX(length) FROM film <br />
WHERE rental_rate=0.99; <br />

4- film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır? <br />
SELECT COUNT(DISTINCT replacement_cost) FROM film <br />
WHERE length>150; <br />
