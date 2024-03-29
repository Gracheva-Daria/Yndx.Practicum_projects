## 🎯 Цель проекта
На основе архива объявлений из сервиса Яндекс.Недвижимость изучить и выявить параметры, влияющие на стоимость квартир в г. Санкт-Петербурге и соседних населённых пунктах.
<hr>

## 📂 Исходные данные для анализа
Расстояние до ближайшего аэропорта в метрах, число балконов, высота потолков, расстояние до центра города, сколько дней было размещено объявление (от публикации до снятия), дата публикации, этаж, всего этажей в доме, апартаменты (булев тип), площадь кухни в квадратных метрах, цена на момент снятия с публикации, жилая площадь в квадратных метрах, название населённого пункта, свободная планировка, число парков в радиусе 3 км, расстояние до ближайшего парка, число водоёмов в радиусе 3 км, расстояние до ближайшего водоёма, число комнат, квартира-студия (булев тип), площадь квартиры в квадратных метрах, число фотографий квартиры в объявлении.
<hr>

## ⌛ В ходе выполнения проекта произвела
Предобработку данных (обработка пропусков, изменение типов данных), расчет и добавление новых данных с характеристиками квартир в датафрейм, исследовательский анализ данных, отсечение аномалий и визуализацию финальных результатов. Сформулировала общий вывод по результатам исследования и дала рекомендации техническим специалистам по улучшению выгрузки данных.
<hr>

## 📃 Общий вывод
**В результате проведенного исследования квартир в центральной части г. Санкт-Петербурга и соседних населенных пунктах были
определены следующие параметры, влияющие на рыночную стоимость квартир:**

1) Площадь квартиры (сильная положительная корреляция).
2) Расположение на этаже (квартиры на 1-ом и на последнем этаже дешевле всех остальных).
3) Экономическая ситуация на рынке в текущем году и курс валют оказывают влияние на изменение цен.

**Были выявлены аномалии, при которых стоит учесть следующее:**

- если продажи прошли меньше, чем за полтора месяца (43 дня) - их можно считать крайне быстрыми.
- если продажи прошли более, чем за 1 год и 2 месяца (460 дней) - их можно считать крайне долгими.

**Выделены города-лидеры (из 10-ти отобранных по кол-ву объявлений) по уровню стоимости квартир:**

1) г. Санкт-Петербург - самый "дорогой" город по стоимости квартир.
2) г. Пушкин - второй по дороговизне город (несмотря на маленькое количество размещенных объявлений).
3) г. Выборг - самый "дешевый" город по стоимости квартир.
<hr>

## 🛠️ Используемые инструменты
`Python`, `Pandas`, `Matplotlib`
