# Ödev 8

* test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.

```sql
CREATE TABLE employee (
	id SERIAL,
	name VARCHAR(50),
	birthday DATE,
	email VARCHAR(100)
);
```

* Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

```sql
insert into employee (id, name, birthday, email) values (1, 'Ichabod', '2023-07-31', 'iclewarth0@eventbrite.com');
insert into employee (id, name, birthday, email) values (2, 'Jessa', '2024-02-29', 'jwelman1@unblog.fr');
insert into employee (id, name, birthday, email) values (3, 'Bernette', '2024-02-14', null);
insert into employee (id, name, birthday, email) values (4, 'Westbrooke', '2023-10-22', 'whuxster3@nature.com');
insert into employee (id, name, birthday, email) values (5, 'Albrecht', '2024-03-23', 'akorbmaker4@4shared.com');
insert into employee (id, name, birthday, email) values (6, 'Carly', '2023-07-15', 'cdobbson5@hc360.com');
insert into employee (id, name, birthday, email) values (7, 'Rem', '2024-03-18', 'rslimmon6@ft.com');
insert into employee (id, name, birthday, email) values (8, 'Virgie', '2024-01-12', null);
insert into employee (id, name, birthday, email) values (9, 'Marc', '2024-04-12', 'mgerwood8@unicef.org');
insert into employee (id, name, birthday, email) values (10, 'Ollie', '2023-11-15', 'ofullwood9@un.org');
insert into employee (id, name, birthday, email) values (11, 'Colette', '2023-04-28', 'cbyrcha@360.cn');
insert into employee (id, name, birthday, email) values (12, 'Bryana', '2024-04-05', 'baltonb@ning.com');
insert into employee (id, name, birthday, email) values (13, 'Damon', '2023-10-06', 'dbowgenc@apache.org');
insert into employee (id, name, birthday, email) values (14, 'Vickie', '2024-01-21', 'vstowted@nature.com');
insert into employee (id, name, birthday, email) values (15, 'Ilse', '2023-05-30', 'ithringe@wufoo.com');
insert into employee (id, name, birthday, email) values (16, 'Caresse', '2023-04-29', 'catleef@amazon.de');
insert into employee (id, name, birthday, email) values (17, 'Spense', '2023-06-12', 'sbeardsellg@paginegialle.it');
insert into employee (id, name, birthday, email) values (18, 'Chryste', '2024-02-08', 'cshailerh@blogspot.com');
insert into employee (id, name, birthday, email) values (19, 'Adelaida', '2024-02-21', 'agraysoni@reference.com');
insert into employee (id, name, birthday, email) values (20, 'Titus', '2024-01-08', null);
insert into employee (id, name, birthday, email) values (21, 'Edgardo', '2023-06-29', 'ehallerk@dailymotion.com');
insert into employee (id, name, birthday, email) values (22, 'Arabele', '2023-12-12', 'ahansterl@foxnews.com');
insert into employee (id, name, birthday, email) values (23, 'Chryste', '2023-05-23', 'clawleym@engadget.com');
insert into employee (id, name, birthday, email) values (24, 'Frederic', '2023-10-17', 'ffersonn@nymag.com');
insert into employee (id, name, birthday, email) values (25, 'Bryce', '2024-02-27', 'bwoodrowo@vkontakte.ru');
insert into employee (id, name, birthday, email) values (26, 'Rudiger', '2023-11-14', 'rrosternp@cam.ac.uk');
insert into employee (id, name, birthday, email) values (27, 'Guthrie', '2024-03-08', 'gespadateq@yahoo.co.jp');
insert into employee (id, name, birthday, email) values (28, 'Paulo', '2024-03-05', 'pgaydonr@netlog.com');
insert into employee (id, name, birthday, email) values (29, 'Bertha', '2023-08-15', 'bleppingtons@wisc.edu');
insert into employee (id, name, birthday, email) values (30, 'Madel', '2023-10-05', 'mbattt@bbc.co.uk');
insert into employee (id, name, birthday, email) values (31, 'Thurstan', '2024-02-13', null);
insert into employee (id, name, birthday, email) values (32, 'Vannie', '2023-12-17', 'vrannv@nyu.edu');
insert into employee (id, name, birthday, email) values (33, 'Anetta', '2023-05-11', 'awebbenw@ebay.co.uk');
insert into employee (id, name, birthday, email) values (34, 'Barron', '2023-08-07', 'bfogtx@digg.com');
insert into employee (id, name, birthday, email) values (35, 'Misti', '2023-08-28', 'mgrishinovy@imdb.com');
insert into employee (id, name, birthday, email) values (36, 'Ardella', '2023-09-13', 'agerbz@eepurl.com');
insert into employee (id, name, birthday, email) values (37, 'Ban', '2023-07-16', 'bsimkovich10@apple.com');
insert into employee (id, name, birthday, email) values (38, 'Josephine', '2023-06-26', 'jquoit11@nature.com');
insert into employee (id, name, birthday, email) values (39, 'Niven', '2023-06-05', 'nmagnar12@about.com');
insert into employee (id, name, birthday, email) values (40, 'Darda', '2024-04-09', 'dreely13@reuters.com');
insert into employee (id, name, birthday, email) values (41, 'Madelon', '2023-07-29', 'mkapelhof14@microsoft.com');
insert into employee (id, name, birthday, email) values (42, 'Broddy', '2024-02-17', 'bgaytor15@icq.com');
insert into employee (id, name, birthday, email) values (43, 'Silvan', '2023-09-26', 'smidden16@about.com');
insert into employee (id, name, birthday, email) values (44, 'Lulu', '2024-02-02', 'lgeraud17@cyberchimps.com');
insert into employee (id, name, birthday, email) values (45, 'Rourke', '2023-12-23', 'rgeke18@networkadvertising.org');
insert into employee (id, name, birthday, email) values (46, 'Kanya', '2024-03-21', null);
insert into employee (id, name, birthday, email) values (47, 'Charlton', '2024-01-01', 'cpratton1a@omniture.com');
insert into employee (id, name, birthday, email) values (48, 'Torrin', '2023-06-12', 'tringham1b@phoca.cz');
insert into employee (id, name, birthday, email) values (49, 'Sheila-kathryn', '2024-04-13', 'spinel1c@netlog.com');
insert into employee (id, name, birthday, email) values (50, 'Raphael', '2023-09-28', 'rtilbey1d@sourceforge.net');
```

* Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

```sql
UPDATE employee
SET 
name = 'guncel_isim',
birthday = '2000-01-01',
email = 'email@yeni.com'
WHERE id < 6 
RETURNING *;
```

* Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

```sql
DELETE FROM employee
WHERE id < 6 
RETURNING *;
```