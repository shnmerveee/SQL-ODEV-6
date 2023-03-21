# SQL-ODEV-6
film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?
ÇÖZÜM: SELECT AVG(rental_rate)FROM film

![5456545645456](https://user-images.githubusercontent.com/128131203/226567857-88a1101a-1dfb-4fd0-9a37-c497cde0c426.PNG)

film tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar?
ÇÖZÜM:SELECT COUNT(title) FROM film
WHERE title LIKE 'C%'

![777777777777](https://user-images.githubusercontent.com/128131203/226569916-ac38a226-ef3e-492e-9913-d9ddf6d7767c.PNG)

film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?
ÇÖZÜM:SELECT* FROM film
WHERE rental_rate= 0.99
ORDER BY length DESC
LIMIT 1

![8888888888](https://user-images.githubusercontent.com/128131203/226570897-7ab8511a-29b6-43ca-8258-c87bd9e9f159.PNG)

film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?
ÇÖZÜM:SELECT COUNT(DISTINCT(replacement_cost)) FROM film
WHERE length >150

![465566546](https://user-images.githubusercontent.com/128131203/226572346-df8a455c-3812-4dea-b462-4f1faa73a9eb.PNG)
