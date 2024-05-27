# -SI_2024_lab2_233295
Драган Бучковски
233295

![cfg](https://github.com/kranoxje/-SI_2024_lab2_233295/assets/165957913/9c96d490-dcb7-4778-9172-2e1c1ea6ec50)




Цикломатската комплексност е 10 бидејќи, бројот на предикатни јазли е 9, односно 9 јазли се разгрануваат, па 9 + 1= 10.

Цикломатската комплексност може да ја пресметаме и како:

број на ребра – број на јазли + 2

број на ребра = 35

број на јазли = 27

35 – 27 = 8 + 2 = 10


![excel](https://github.com/kranoxje/-SI_2024_lab2_233295/assets/165957913/f455bf1b-663d-469b-bb1b-0955848143d4)



Прв тест случај: allItems = null, payment = 6000

Во овој случај, бидејќи allItems е null ќе влезе во if (allItems == null) и веднаш ќе фрли RuntimeExecption и ќе заврши програмата.

Втор тест случај: allItems = [bread, milk, null], payment = 6000

Barcode: Price: Discount

bread: 563218 bread: 100 bread: 0

milk: 084579 milk: 520 milk: 10

null: 42a5c6 null: 400 null: 0

Во овој тест, го опфаќам случајот каде allItems содржи производ кој нема име (null) и исто така allItems содржи производ кој започнува на „0” и производ кој во баркодот има карактер. Поради тоа, програмата ќе заврши со Invalid character in item barcode!

Трет тест случај: allItems = [bread, milk, water], payment = 6000

Barcode: Price: Discount

bread: 563218 bread: 300 bread: 0

milk: 084579 milk: 620 milk: 10

water: water: 290 water: 15

Во овој тест, го опфаќам случајот каде allItems содржи производ кој нема баркод, така што ќе фрли исклучок со порака „No barcode”. Поради исклучокот, програмата ќе заврши и нема можност за печатење на сумата.

Четврт тест случај: allItems = [bread, milk, cheese], payment = 6000

Barcode: Price: Discount

bread: 563218 bread: 300 bread: 0

milk: 084579 milk: 620 milk: 10

cheese: 28637 cheese: 480 cheese: 15

Во овој тест, сите производи од листата allItems се валидни и на крај добиваме sum > payment со што програмата враќа false.

Петти тест случај: allItems = [bread, milk, cheese], payment = 6000

Barcode: Price: Discount

bread: 563218 bread: 300 bread: 5

milk: 084579 milk: 320 milk: 10

cheese: 28637 cheese: 200 cheese: 3

Во овој тест, сите производи од листата allItems се валидни и на крај добиваме sum < payment со што програмата враќа true.
