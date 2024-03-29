### ✅ Корректное отображение тетради проекта (а именно графиков-воронок из библиотеки Plotly) доступно в Jupyter NBViewer [по этой ссылке.](https://nbviewer.jupyter.org/github/Gracheva-Daria/Yndx.Practicum_projects/blob/main/09_%D0%98%D1%81%D1%81%D0%BB%D0%B5%D0%B4%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5%20%D0%BF%D0%BE%D0%B2%D0%B5%D0%B4%D0%B5%D0%BD%D0%B8%D1%8F%20%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D0%B5%D0%B9%20%D0%BC%D0%BE%D0%B1%D0%B8%D0%BB%D1%8C%D0%BD%D0%BE%D0%B3%D0%BE%20%D0%BF%D1%80%D0%B8%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D1%8F%20%D0%B8%20%D1%80%D0%B5%D0%B7%D1%83%D0%BB%D1%8C%D1%82%D0%B0%D1%82%D0%BE%D0%B2%20AAB-%D1%82%D0%B5%D1%81%D1%82%D0%B0/09_%D0%98%D1%81%D1%81%D0%BB%D0%B5%D0%B4%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5%20%D0%BF%D0%BE%D0%B2%D0%B5%D0%B4%D0%B5%D0%BD%D0%B8%D1%8F%20%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D0%B5%D0%B9%20%D0%BC%D0%BE%D0%B1%D0%B8%D0%BB%D1%8C%D0%BD%D0%BE%D0%B3%D0%BE%20%D0%BF%D1%80%D0%B8%D0%BB%D0%BE%D0%B6%D0%B5%D0%BD%D0%B8%D1%8F%20%D0%B8%20%D1%80%D0%B5%D0%B7%D1%83%D0%BB%D1%8C%D1%82%D0%B0%D1%82%D0%BE%D0%B2%20AAB-%D1%82%D0%B5%D1%81%D1%82%D0%B0.ipynb)
<hr>

## 🎯 Цель проекта
Выявить особенности поведения пользователей приложения магазина продуктов питания и проанализировать результат А/А/В-теста для определения влияния экспериментальных новых шрифтов приложения на конверсию пользователей в покупатели.
<hr>

## 📂 Исходные данные для анализа
**Датасет с логами (каждая запись в логе — это действие пользователя, или событие).**

**Датасет содержит:** название события; уникальный идентификатор пользователя; время события; номер эксперимента: 246 и 247 — контрольные группы, а 248 — экспериментальная.
<hr>

## ⌛ В ходе выполнения проекта произвела
Предобработку данных (изменение типов данных, обработка дубликатов), исследовательский анализ данных с визуализацией результатов, исключение не актуального периода, формирование и анализ воронки событий, анализ конверсии, проверку 4-х статистических гипотез о различии долей между группами A/A/B-теста. По результатам исследования сформулировала общий вывод с рекомендациями.
<hr>

## 📃 Общий вывод
**В результате проведённого исследования определено следующее:**
1. Исходные данные были предоставлены за период 2 недели: с 25 Июля 2019 по 07 Августа 2019, 1 неделя из которых неполная и была исключена из дальнейшего анализа. Актуальный период, который мы изучили: с 01 Августа 2019 по 07 Августа 2019 (7 дней).
2. Из 5 возможных событий (`Main Screen Appear`, `Offers Screen Appear`, `Cart Screen Appear`, `Payment Screen Successful` и `Tutorial`) чаще всего встречается событие `Main Screen Appear` - 48,7% от всех событий.
3. Событие `Tutorial` для анализа конверсии пользователей не играет роли и было исключено из воронки событий.
4. Все 5 событий совершили только 6% уникальных пользователей.
5. Только 1 событие совершили 36% пользователей (`MainScreenAppear` или `OffersScreenAppear` или `Tutorial`).
6. Только 61,9% доходят до экрана с предложениями товара (событие `Offers Screen Appear`) и, соответственно, 38,1% потенциальных покупателей магазин теряет уже при переходе на 2-ой этап.
7. До события `Cart Screen Appear` не доходят еще 18% пользователей.
8. 5,2% пользователей после события `Cart Screen Appear` не завершают покупку.
9. 47.70% пользователей проходят всю воронку событий.
10. По результатам проведённого А/А/В - теста не выявлено статистически значимых различий в конверсии, что говорит о том, что **внедрение в приложение дизайнерами новых шрифтов не повлияло на конверсию пользователей.**

 **Рекомендации:**
Т.к. актуальные данные оказались только за 1 неделю можно продолжить сбор данных по 3-м экспериментальным группам. Но из-за достаточно высоких показателей P-value и множественных проверок вероятность получить статистически значимые отличия долей в группах по окончанию сбора данных представляется крайне низкой. Рекомендуется разработать новые гипотезы и провести их приоритизацию с дальнейшим тестированием.
<hr>

## 🛠️ Используемые инструменты
`Python`, `Pandas`,` NumPy`, `Matplotlib`, `Plotly`, `Math`, `SciPy`, `Z-критерий`
