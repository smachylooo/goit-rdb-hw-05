# Домашнє завдання 5 — Смачило Богдан Андрійович

## Google Colab

**[Відкрити домашнє завдання в Google Colab](https://colab.research.google.com/drive/1d5_62J_sxj_36zI74qAQZdvcbJgPpQ2A?usp=sharing)**

## Опис

Домашня робота присвячена роботі з PostgreSQL і датасетом Olist: створенню типізованих таблиць, підготовці ознак для аналізу та оптимізації SQL-запитів.

## Завдання

1. Налаштування PostgreSQL, завантаження Olist і створення typed-схеми.
2. CTE-chain pipeline для обчислення ознак клієнтів (RFM, cohort, rolling AOV, cancellation rate, preferred category).
3. Recursive CTE для аналізу referral chain із захистом від циклів.
4. Materialized View та `REFRESH MATERIALIZED VIEW CONCURRENTLY`.
5. Порівняння запитів через `EXPLAIN (ANALYZE, BUFFERS)` і висновки (Reflection).

## Як запустити

1. Перейдіть за посиланням на Google Colab вище.
2. За потреби створіть власну копію блокнота: **File → Save a copy in Drive**.
3. Запускайте клітинки послідовно зверху вниз через **Runtime → Run all**.
4. Для роботи з повним датасетом Olist може знадобитися доступ до Kaggle або CSV-файли з курсового архіву. Якщо використовується навчальна stub-схема, це слід зазначити в результатах.

## Технології

- Python, pandas
- PostgreSQL, SQLAlchemy, psycopg2
- Google Colab / Jupyter Notebook

## Примітка

Результати виконання SQL і плани `EXPLAIN ANALYZE` залежать від фактично завантажених даних та середовища запуску.
