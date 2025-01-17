# goit-algo-hw-05
Search algorithms

ЗАВДАННЯ 3
========================================

Порівняння ефективності алгоритмів пошуку підрядка: Боєра-Мура (БМ), Кнута-Морріса-Пратта (КМП) та Рабіна-Карпа (РК) на основі двох текстових файлів (Стаття 1, Стаття 2).

****************************************
**РЕЗУЛЬТАТИ**
========================================

Стаття 1
----------------------------------------
URL статті: https://drive.google.com/uc?export=download&id=18_R5vEQ3eDuy2VdV3K5Lu-R-B-adxXZh
- -- -- -- -- -- -- -- -- -- -
Підрядок існуючий: поширена дія

КМП: 0.5149664000000485 сек
Індекс: 2560
- - - - 
БМ: 0.1894496999993862 сек
Індекс: 2560
- - - - 
РК: 1.210005299999466 сек
Індекс: 2560
- -- -- -- -- -- -- -- -- -- -
Підрядок вигаданий: How are you?

КМП: 1.9200909000010142 сек
Індекс: -1
- - - - 
БМ: 0.5410155999998096 сек
Індекс: -1
- - - - 
РК: 5.8341734999994515 сек
Індекс: -1

****************************************

Стаття 2
----------------------------------------
URL статті: https://drive.google.com/uc?export=download&id=13hSt4JkJc11nckZZz2yoFHYL89a4XkMZ
- -- -- -- -- -- -- -- -- -- -
Підрядок існуючий: Метою даної роботи є

КМП: 0.055259900000237394 сек
Індекс: 220
- - - - 
БМ: 0.014402999999219901 сек
Індекс: 220
- - - - 
РК: 0.18002725904807448 сек
Індекс: 220
- -- -- -- -- -- -- -- -- -- -
Підрядок вигаданий: How are you?

КМП: 2.7743098999999347 сек
Індекс: -1
- - - - 
БМ: 0.8409503000002587 сек
Індекс: -1
- - - - 
РК: 11.417079700000613 сек
Індекс: -1

****************************************
**ВИСНОВКИ**
========================================

Висновки до Статті 1
----------------------------------------
1. Для існуючого підрядка "поширена дія" найшвидшим виявився алгоритм Боєра-Мура (0.19 сек), який значно випередив КМП (0.51 сек) та РК (1.21 сек).
2. Всі алгоритми знайшли підрядок на однаковому індексі (2560).
3. При пошуку неіснуючого підрядка "How are you?" алгоритм БМ також показав найкращий результат (0.54 сек).

Висновки до Статті 2
----------------------------------------
1. При пошуку існуючого підрядка "Метою даної роботи є" алгоритм БМ знову показав найкращий результат (0.014 сек).
2. Всі алгоритми знайшли підрядок на індексі 220.
3. При пошуку неіснуючого підрядка алгоритм БМ залишився найефективнішим (0.84 сек).

Загальні висновки
----------------------------------------
1. Алгоритм Боєра-Мура стабільно показує найкращу продуктивність на обох текстах.
2. Алгоритм Рабіна-Карпа виявився найповільнішим у всіх тестах.
3. КМП показує середні результати, але значно поступається алгоритму БМ.
4. При пошуку неіснуючого підрядка час виконання всіх алгоритмів значно збільшується.