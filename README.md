# sqlodev6
sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.

1-)film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?
select AVG(rental_rate) FROM film;
2-)film tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar?
select COUNT(*) FROM film where title LIKE 'C%';
3-)film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?
select MAX(length) from film where rental_rate = 0.99 ;
4-)film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır?
select COUNT( DISTINCT replacement_cost ) from film where length>150;
