# Osnovi_Proektirovania_BD
1.2 SQL
1) SELECT * FROM book;
2)SELECT author, title, price FROM book;
3) SELECT title AS Название, author as Автор 
FROM book;
4)SELECT title, amount, 
 1.65 * amount as pack 
 FROM book 
5)SELECT title, author , amount , 
 ROUND ((price-price/100*30),2) AS new_price 
FROM book; 
6)SELECT author,title, 
 ROUND (if(author = 'Булгаков М.А.', price * 1.1, 
if (author = 'Есенин С.А.', price * 1.05, price)),2) AS new_price 
FROM 
 book; 
7)SELECT author, title, price 
FROM book 
WHERE amount<10; 
8)SELECT title, author, price, amount 
FROM book 
WHERE amount = 15; 
9)SELECT title, author 
FROM book 
WHERE price BETWEEN 540.50 AND 800 AND amount IN(2 , 3 , 5 , 7); 
10)SELECT author, title 
FROM book 
WHERE amount between 2 and 14 
ORDER BY author DESC , title asc ; 
11)SELECT title, author 
FROM book 
WHERE title LIKE "_% _%" and author LIKE "_% %С.%" 
order by title asc; 
12)SElECT * 
FROM book 
 
