# https-app.patika.dev-courses-sql-Odev4

--film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız
SELECT DISTINCT replacement_cost FROM film;

--film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?
SELECT COUNT (DISTINCT replacement_cost) FROM film;
--21 farklı veri vardır.

--film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?
SELECT COUNT (title) FROM film 
WHERE title LIKE 'T%' AND rating='G';
--9
