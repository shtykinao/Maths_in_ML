## Лабораторная работа № 4
## Многомерный анализ данных для улучщения их качества

**Цель работы** - использовать методы многомерного анализа данных для улучшения качества работы модели машинного обучения. 

В данной лабораторной работе решается та же задача, что и в [лабораторной работе № 3](https://github.com/shtykinao/Maths_in_ML/tree/main/lab3). 

### Ход работы:
- Для выявления зависимостей между признаками была построена корреляционная матрица; 
- Был использован VIF анализ для обнаружения мультиколлинеарности среди предикторов; 
- Был проведен кластерный анализ для выявления естественных группировок в данных;  
- Были сгенерированы дополнительные признаки как полиномиальные (степень 3) комбинации исходных, а также был произведен их отбор с помощью регуляризационного метода Lasso;
- Была обучена структура байесовской сети с помощью алгоритма Hill-Climbing, далее сеть была использована для отбора переменных, создания синтетических данных и балансировки классов; 
- Была повторна обучена модель на новых датасетах, полученные метрики были проанализированы.

### Результаты:
Наилучшие результаты показало применение байесовской сети.  Дополнительное создание признаков и их последующий отбор изменило структуру признаков датасета, что добавило гибкости модели, но привело к ухудшению целевых результатов обучения. 