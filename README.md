# DS_Taxi_strategy

## Тема:
«Формирование стратегии крупного агрегатора такси (поиск инсайтов, проверка гипотезы, составление рекомендаций стейкхолдерам, построение предиктивной модели)».

## Цель задания:
- Собрать все полученные на курсе знания воедино.
- Закрепить умение исследовать данные, проверять гипотезу, делать выводы и презентовать результаты.
- Закрепить умение исследовать внешние факторы, строить модель, получать прогноз и делать выводы.

## Подготовка среды
Виртуальное окружение:
```bash
sudo apt update
sudo apt install python3.10-venv
python3 -m venv .venv
```
Активация виртуального окружения:
```bash
source .venv/bin/activate
```
Установка необходимых библиотек:
```bash
pip3 install numpy pandas matplotlib scipy
```

## Задание:
### Введение:
Поздравляем! Вы попали на стажировку в одно из подразделений группы компаний, Вы — аналитик крупного агрегатора такси. Теперь перед вами стоит важная задача: самостоятельно провести исследование данных, проверить гипотезу о поведенческом предпочтении пользователей к определённому классу такси и сделать выводы, чтобы помочь компании стать лучшей на рынке. Успехов!


### 1	Загрузите файл dip_hw_x_taxi.csv в pandas dataframe
### 2	Рассчитайте основные описательные статистики (среднее, минимум, 25-50-75-персентили, максимум)
### 3	Вычислите количество значений по классам такси
### 4	Визуализируйте распределение дистанций поездок
### 5	Визуализируйте распределения дистанций поездок, по каждому классу такси в отдельности, а также определите типы распределений для эконом-класса и комфорт-класса
### 6	Сформируйте выборки по эконом и комфорт-классам. Визуализируйте пересечение интервалов дистанций этих классов 
(примечание: поможет функция seaborn.distplot или seaborn.kdeplot)
### 7	Проведите стат. тест 
(поможет: функция scipy.stats.ttest_ind), проверьте гипотезу, что дистанции поездок в комфорт-классе отличаются от дистанций поездок эконом-класса (примечание: H0 – выборки не отличаются, H1 – выборки отличны; уровень значимости = 5%)
### 8	Сделайте выводы по результатам проведения стат. теста
### 9	Вычислите средние выборок исследуемых классов, с учётом полученного результата проверки гипотез определите – какой из классов предпочитают на дальние поездки (эконом или комфорт)
### 10	Оформите презентацию для демонстрации результатов стейкхолдерам (примечание: для оформления воспользуйтесь шаблоном)


## Вопросы:

1. Как распределяется количество поездок по дням недели? По часам? По часам в будни и в выходные? 

*Найти в какой день недели больше/меньше всего поездок? В какие часы?
В какие дни и часы наблюдается пик спроса на такси?*

2. Как распределяются поездки по классам? 

*Определить количество поезок каждого из них.
Какие классы поездок (Economy, Comfort, Premium, Delivery) наиболее популярны?*

3. В какой день / час больше или меньше всмего поездок для каждого класса?

*Выявить закономерности по периодам времени поездок по каждому классу сервиса.*

4. Какое среднее расстояние поездки для каждого класса?

   *Выявить закономерности в длине поездок по каждому классу сервиса.*

5. Каково отношение количества отмененных поездок ко всем поездкам? 

6. Поездки какого класса чаще всего отменяют? А в процентном соотношении по классам? 
*Есть ли зависимости между классом поездки и вероятностью ее отмены?*

7. Как меняется количество отмен относительно длины поездки? А для каждого класса? 

8. Какие закономерность между отменами поездок и дистанцией?

