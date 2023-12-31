# AB-testing
Smart Discount Strategy

# Описание

В данном проекте проводится A/B тестирование для проверки эффективности удержания аудитории на сервисе скидок с помощью скидки 1% на следующий период подписки. Основной инструмент проверки - непараметрический тест Манна-Утни, поскольку разница длительности между старой и новой подписками по Колмагорову тесту оказалась ненормально распределенной. Далее был проведен продвинутый AAB- тест на основе разбивки на две контрольные группы и одну тестовую. Получившиеся pvalue были скорректированы помощью метода Холма для контроля над ложноположительными результатами.

# Результаты:

При проведении обоих AB-тестов тестов были получены высокие pvalue, что означает, что статистически значимых различий в распределениях между контрольной и тестовой группами не наблюдается. После коррекции Холма p-значения даже увеличились, подтверждая предыдущий вывод. Следовательно, добавление скидки не оказало значительного влияния.

# Использованные технологии:

python, pandas, numpy, seaborn, matplotlib, scipy.stats, statmodels, kstest, mannwhitneyu, ttest_ind, multipletests
