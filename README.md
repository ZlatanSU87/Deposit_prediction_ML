![](https://yandex-images.clstorage.net/5CVP0U233/3517bdnsx/Wx1d2r_Ug-isle563IZEUNsI3GWTQqaW5Ry6m6L3zghvtMoe51mOqKA2y8XK_FxRJP7QSuYh4nS9waNjVW4XbBdQDZ-OyYeF3cD2J4ymSETTfalp1zPOh5F1s-rys_tQQ6znuh_UWjkdw09xWxDxaEXWkBNPuba9CAlinnTD1sULDY2if9AC_JBdCyZ8vmzcW91wnYuvIh_VtEPSfrYzNWrFz3KvkFq1NXc3baNweQB80vz3v3yC9RDldqowg1Ydk4XdAmswAsDwDbcGgLqoHO_NwFFve7a73Vij1oI2d_V2gY_Cx2QKuVVjx_WHuGWkiKZ4IxeQ1m3wQdJWNMeCFZMlfZIHDOqE0OX3BoQSlADr2QyZl6MG61ksL-rSpt_5PmE3AjOU5rmx36fxwwRdbChinPtv7BoVRIGGopjD2lnXgWXWe4BKgFhBb6bwLiig99XchRPz0ruJLPti2r6zfWpFhyY3gG6NpSMr6dPc4Thgcginq2Ci3WABgmpYA5aF18EN3v8kxpT4jadWiIbwbIutsM0zvx6bLTSbYvJGO-UWCa_OJ-RCIW3bJ81DVM3oaPbsIwfkXjGU4SZqyJcGoQulccpfVB5EqIl_TnxmeHwr1dxB508K6_mcT95SQpslZgH7IrNgvnWxx1ORh1zlFBDSbIsfzCL1aL3u1ixDihFH2WGu60h6dDDZA-I0pmzsx43ETdvP8us1nGs-zlIvDSbJk1ZPNEod7UNTUesYHaio6uRfN1Ru1fRtYm4IQ57ZN0EBoneA4mSUwQMm_K5ADFNBDB2Dh7rjpRSbjoZeV8FqvQcSt1g6ITnjlx1rnE2UJCYw59v4CkUYFZKywAOCwX8FzSrnPF7MTAGn3lDCnCAvNaD5C4smU3mcM6pClg_xPilPpkPknpWhT8O9cwxtqMxaVC-bJIZ5DEGOMigHzonTfW3SDxDitAzZvwocQrgAC6W06Q-bhtdB4MtCdsI0)
# <center> Предсказание депозитарной активности клиентов банка
## <center> Оглавление
1. [Опиcание проекта](#описание-проекта)
2. [Описание данных](#описание-данных)
3. [Авторы](#авторы)
4. [Выводы](#выводы)

## Описание проекта
**Дана** [база данных клиентов банка](https://lms-cdn.skillfactory.ru/assets/courseware/v1/dab91dc74eb3cb684755123d224d262b/asset-v1:SkillFactory+DST-3.0+28FEB2021+type@asset+block/bank_fin.zip) в формате **CSV**. 
**Проблематика**: Банкам хотелось бы уметь выбирать среди своих клиентов именно тех, которые с наибольшей вероятностью **откроют депозит**.

Необходимо проанализировать данные, выявить закономерности и найти решающие факторы, повлиявшие на то, что клиент вложил деньги именно в этот банк. Успешное решение этой задачи поднимет доходы банка и поможете понять целевую аудиторию, которую необходимо привлекать путём рекламы и различных предложений.

### Данный проект реализует:
* Первичную обработку данных
* Разведывательный анализ данных (EDA)
* Отбор и преобразование признаков
* Решение задачи классификации: логистическая регрессия и решающие деревья
* Решение задачи классификации: ансамбли моделей и построение прогноза

**О структуре проекта:**
* [plotly](./plotly) - папка с изображениями графиков проекта
* [Deposit_prediction_ML.ipynb](./Deposit_prediction_ML.ipynb) - jupyter-ноутбук, содержащий основной код проекта, в котором демонстрируются методы и подходы решения задачи

## Описание данных
### Данные представляют из себя таблицу со следующими **признаками**:
 Данные о клиентах банка:
* age (возраст);
* job (сфера занятости);
* marital (семейное положение);
* education (уровень образования);
* default (имеется ли просроченный кредит);
* housing (имеется ли кредит на жильё);
* loan (имеется ли кредит на личные нужды);
* balance (баланс).
Данные, связанные с последним контактом в контексте текущей маркетинговой кампании:
* contact (тип контакта с клиентом);
* month (месяц, в котором был последний контакт);
* day (день, в который был последний контакт);
* duration (продолжительность контакта в секундах).
Прочие признаки:
* campaign (количество контактов с этим клиентом в течение текущей кампании);
* pdays (количество пропущенных дней с момента последней маркетинговой кампании до контакта в текущей кампании);
* previous (количество контактов до текущей кампании)
* poutcome (результат прошлой маркетинговой кампании).
* **deposit** - целевая переменная, которая определяет, согласится ли клиент открыть депозит в банке. Именно её мы будем пытаться предсказать в данном кейсе.

**Всего 11162 строк и 17 колонн**

## Используемые зависимости
* Python (3.9.10):
    * [numpy (1.20.3)](https://numpy.org)
    * [pandas (1.3.4)](https://pandas.pydata.org)
    * [matplotlib (3.4.3)](https://matplotlib.org)
    * [seaborn (0.11.2)](https://seaborn.pydata.org)

## Установка проекта

```
git clone https://github.com/ZlatanSU87/Deposit_prediction_ML
```

## Использование
Вся информация о работе представлена в jupyter-ноутбуке Project-4._Ноутбук-шаблон.ipynb.

## Авторы

* [Sergey](https://t.me/IZ20112022)

## Выводы

По итогам обучения модели различными методами можно сделать **вывод**, что **наилучший результат** показывают **градиентный бустинг и случайный лес**, вместе с тем, **метрики отличаются незначительно** в сравнении с остальными моделями. Вероятнее всего дело в том, что окончательная **выборка данных оказалась небольшой** и более продвинутые методы машинного обучения не могут полностью реализовать свой ресурс.