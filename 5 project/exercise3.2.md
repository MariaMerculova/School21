**XPath'ы**

**1. Каждой кнопки:**

#### Выбор полиса

1. //button[@id="mat-button-toggle-1-button"] - квартира  

2. //button[@id="mat-button-toggle-2-button"] - дом

3. //button[@id="mat-button-toggle-49-button"] - сдается в аренду - ДА

4. //button[@id="mat-button-toggle-50-button"] - сдается в аренду - НЕТ

5. //button[@id="mat-button-toggle-52-button"] - Расположена на первом или последнем этаже - ДА

6. //button[@id="mat-button-toggle-53-button"] - Расположена на первом или последнем этаже - НЕТ

7. //button[@id="mat-button-toggle-55-button"] - Установлена охранная сигнализация - ДА

8. //button[@id="mat-button-toggle-56-button"] - Установлена охранная сигнализация - НЕТ

9. //button[@class='mat-focus-indicator action-back mat-stroked-button mat-button-base'] - кнопка Применить

10. //button[@class='mat-focus-indicator mat-stroked-button mat-button-base mat-accent'] - Оформить

#### Оформление

1. //button[@class='mat-focus-indicator sber-id-button mat-flat-button mat-button-base mat-primary'] - кнопка Заполнить по Сбер ID

2. //button[@id='mat-button-toggle-58-button'] - кнопка Мужской

3. //button[@id='mat-button-toggle-59-button'] - кнопка Женский

4. //button[@class='mat-focus-indicator action-back mat-stroked-button mat-button-base'] - кнопка Вернуться

5. //button[@class='mat-focus-indicator mat-flat-button mat-button-base mat-accent'] - кнопка Оформить


    **2. Каждого поля для ввода текста**

    1. //div[@class="mat-form-field-infix ng-tns-c61-0"] - регион проживания

    2. //div[@class="mat-form-field-infix ng-tns-c61-2"] - окно ввода Промокод

    3. //div[@class='mat-form-field-infix ng-tns-c61-3'] - фамилия

    4. //div[@class='mat-form-field-infix ng-tns-c61-4'] - имя

    5. //div[@class='mat-form-field-infix ng-tns-c61-5'] - отчество

    6. //div[@class='mat-form-field-infix ng-tns-c61-6'] - дата рождения

    7. //div[@class='mat-form-field-infix ng-tns-c61-7'] - паспортные данные - серия

    7. //div[@class='mat-form-field-infix ng-tns-c61-8'] - паспортные данные - номер

    9. //div[@class='mat-form-field-infix ng-tns-c61-9'] - паспортные данные - дата выдачи

    10. //div[@class='mat-form-field-infix ng-tns-c61-10'] - паспортные данные - кем выдан

    11. //div[@class='mat-form-field-infix ng-tns-c61-11'] - паспортные данные - код подразделения

    12. //div[@class="mat-form-field-infix ng-tns-c61-13"] - адрес имущества - город или населенный пункт

    13. //div[@class="mat-form-field-infix ng-tns-c61-14"] - адрес имущества - улица

    14. //div[@class="mat-form-field-infix ng-tns-c61-15"] - адрес имущества - дом

    15. //div[@class="mat-form-field-infix ng-tns-c61-16"] - адрес имущества - квартира

    16. //div[@class="mat-form-field-infix ng-tns-c61-17"] - Контактные данные Страхователя - телефон

    17. //div[@class="mat-form-field-infix ng-tns-c61-18"] - Контактные данные Страхователя - эл. почта

    18. //div[@class="mat-form-field-infix ng-tns-c61-19"] - Контактные данные Страхователя - повтор эл. почты

**3. Каждого чекбокса**

        1. //input[@id="mat-checkbox-1-input"] - чекбокс Отчество отсутствует

        2. //input[@id="mat-checkbox-2-input"] - чекбокс Улица отсутствует

**4. Каждого датапикера**

1. //div[@class='mat-form-field-infix ng-tns-c61-21'] - Срок действия страхования - дата

2. //div[@class='mat-form-field-infix ng-tns-c61-26'] - Страхователь - дата рождения

3. //div[@class='mat-form-field-infix ng-tns-c61-29'] - Паспортные данные Страхователя - дата выдачи

**5. Логотипа "СБЕР СТРАХОВАНИЕ"**

//div[@class='sber-logo']

**6. Слайдера в блоке выбора суммы**

//div[@class='mat-slider-thumb']

//div[@class='mat-slider-wrapper']

**7. Хедера "Что будет застраховано?"**

//h4[@class='block-header'][1]

**8. Текстовых блоков:**

**"Мебель, техника и ваши вещи"** 

//div[text()[contains(.,'Мебель, техника и ваши вещи')]]

**"Падение летательных аппаратов и их частей"**

//div[text()[contains(.,'Падение летательных аппаратов и их частей')]]

**9. Каждой колонки в списка, который находится под хедером "Страховая защита включенная в программу".**

Левая колонка - //div[text( )='Чрезвычайная ситуация']/ancestor::ul

Правая колонка - //div[text( )='Стихийные бедствия']/ancestor::ul


