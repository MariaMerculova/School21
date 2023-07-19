## Тест-кейс №1 — Прохождение авторизации под логином "standard_user"
1. Предшествующие условия:
    - открыта страница авторизации сайта https://www.saucedemo.com/
2. Шаги:
    - ввести Имя пользователя "standard_user"
    - ввести Пароль "secret_sauce"
    - нажать на кнопку "Login"
3. Ожидаемый результат:
    - при нажатии на кнопку "Login", пользователь будет успешно авторизован

## Тест-кейс №2 — Прохождение авторизации под логином "locked_out_user"
1. Предшествующие условия:
    - открыта страница авторизации сайта https://www.saucedemo.com/
2. Шаги:
    - ввести Имя пользователя "locked_out_user"
    - ввести Пароль "secret_sauce"
    - нажать на кнопку "Login"
3. Ожидаемый результат:
    - при нажатии на кнопку "Login", пользователь будет успешно авторизован

## Тест-кейс №3 — Прохождение авторизации под логином "problem_user"
1. Предшествующие условия:
    - открыта страница авторизации сайта https://www.saucedemo.com/
2. Шаги:
    - ввести Имя пользователя "problem_user"
    - ввести Пароль "secret_sauce"
    - нажать на кнопку "Login"
3. Ожидаемый результат:
    - при нажатии на кнопку "Login", пользователь будет успешно авторизован

## Тест-кейс №4 — Прохождение авторизации под логином "performance_glitch_user"
1. Предшествующие условия:
    - открыта страница авторизации сайта https://www.saucedemo.com/
2. Шаги:
    - ввести Имя пользователя "performance_glitch_user"
    - ввести Пароль "secret_sauce"
    - нажать на кнопку "Login"
3. Ожидаемый результат:
    - при нажатии на кнопку "Login", пользователь будет успешно авторизован

## Тест-кейс №5 — Нажатие кнопки "Добавить в Корзину"
1. Предшествующие условия:
    - пользователь авторизован
    - открыта главная страница магазина
2. Шаги:
    - навести курсор на запись "Добавить в Корзину"
    - нажать на кнопку "Добавить в корзину"
3. Ожидаемый результат:
    - при нажатии на кнопку "Добавить в корзину", товар добавляется в корзину
    - кнопка "Добавить в корзину", заменяется на кнопку "Удалить"
    - к значку "Корзина" добавляется количество добавленных товаров

## Тест-кейс №6 — Нажатие иконки "Корзина"
1. Предшествующие условия:
    - пользователь авторизован
    - открыта главная страница магазина
2. Шаги:
    - навести курсор на иконку "Корзина" 
    - нажать на иконку "Корзина"
3. Ожидаемый результат:
    - при нажатии на иконку "Корзина" открывается корзина с выбранным товаром

## Тест-кейс №7 — Нажатие на картинку "карточка товара"
1. Предшествующие условия:
    - пользователь авторизован
    - открыта главная страница магазина
2. Шаги:
    - навести курсор на картинку "карточка товара"
    - нажать на картинку "карточка товара"
3. Ожидаемый результат:
    - при нажатии на картинку "карточка товара", откроется новая страница с описанием товара

## Тест-кейс №8 — Нажатие кнопки "Фильтр Название (от А до Я)"
1. Предшествующие условия:
    - пользователь авторизован
    - открыта главная страница магазина
2. Шаги:
    - навести курсор на запись
    - нажать на кнопку "Фильтр" Название (от А до Я)
3. Ожидаемый результат:
    - при нажатии на кнопку "Фильтр" Название (от А до Я), открывается окно с выбором сортировки

## Тест-кейс №9 — Нажатие кнопки "Фильтр Название (от А до Я)"
1. Предшествующие условия:
    - пользователь авторизован
    - открыта главная страница магазина
2. Шаги:
    - навести курсор на запись
    - нажать на кнопку "Фильтр" Название (от А до Я)
    - выбрать и нажать на кнопку "Фильтр" Название (от А до Я)
3. Ожидаемый результат:
    - при нажатии на кнопку "Фильтр" Название (от А до Я), товар отсортируется по алфавиту

## Тест-кейс №10 — Нажатие кнопки "Фильтр Название (от Я до А)"
1. Предшествующие условия:
    - пользователь авторизован
    - открыта главная страница магазина
2. Шаги:
    - навести курсор на запись
    - нажать на кнопку "Фильтр" Название (от А до Я)
    - выбрать и нажать на кнопку "Фильтр" Название (от Я до А)
3. Ожидаемый результат:
    - при нажатии на кнопку "Фильтр" Название (от Я до А), товар отсортируется в обратном порядке алфавита

## Тест-кейс №11 — Нажатие кнопки Фильтр "Цена (от низкой до высокой)"
1. Предшествующие условия:
    - пользователь авторизован
    - открыта главная страница магазина
2. Шаги:
    - навести курсор на запись
    - нажать на кнопку "Фильтр" Название (от А до Я)
    - навести курсор на запись "Цена (от низкой до высокой)"
    - нажать на кнопку "Цена (от низкой до высокой)"
3. Ожидаемый результат:
    - при нажатии на кнопку "Цена (от низкой до высокой)", товар отсортируется по возрастанию

## Тест-кейс №12 — Нажатие кнопки Фильтр "Цена (от высокой до низкой)"
1. Предшествующие условия:
    - пользователь авторизован
    - открыта главная страница магазина
2. Шаги:
    - навести курсор на запись
    - нажать на кнопку "Фильтр" Название (от А до Я)
    - навести курсор на запись "Цена (от высокой до низкой)"
    - нажать на кнопку "Цена (от высокой до низкой)"
3. Ожидаемый результат:
    - при нажатии на кнопку "Цена (от высокой до низкой)", товар отсортируется от большей стоимости товара до меньшей стоимости товара

## Тест-кейс №13 — Нажатие кнопки Меню (три горизонтальные полоски)
1. Предшествующие условия:
    - пользователь авторизован
    - открыта главная страница магазина
2. Шаги:
    - навести курсор на Меню (три полоски)
    - нажать на кнопку Меню (три полоски)
3. Ожидаемый результат:
    - при нажатии на кнопку "Меню (три полоски)", откроется окно с вкладками "Все товары", "О нас", "Выход","Сбросить состояние приложения"

## Тест-кейс №14 — Нажатие кнопки "Все товары" в открытом Меню
1. Предшествующие условия:
    - пользователь авторизован
    - открыта главная страница магазина
    - открыто Меню
2. Шаги:
    - навести курсор на Меню (три полоски)
    - нажать на кнопку Меню (три полоски)
    - навести курсор на кнопку "Все товары"
    - нажать на кнопку "Все товары"
3. Ожидаемый результат:
    - при нажатии на кнопку "Все товары", откроется перечень товаров на главное странице

## Тест-кейс №15 — Нажатие кнопки "О нас" в открытом Меню
1. Предшествующие условия:
    - пользователь авторизован
    - открыта главная страница магазина
    - открыто Меню
2. Шаги:
    - навести курсор на Меню (три полоски)
    - нажать на кнопку Меню (три полоски)
    - навести курсор на кнопку "О нас"
    - нажать на кнопку "О нас"
3. Ожидаемый результат:
    - при нажатии на кнопку "О нас", откроется новая страница с описанием интернет-магазина

## Тест-кейс №16 — Нажатие кнопки "Выход" в открытом Меню
1. Предшествующие условия:
    - пользователь авторизован
    - открыта главная страница магазина
    - открыто Меню
2. Шаги:
    - навести курсор на Меню (три полоски)
    - нажать на кнопку Меню (три полоски)
    - навести курсор на кнопку "Выход"
    - нажать на кнопку "Выход"
3. Ожидаемый результат:
    - при нажатии на кнопку "Выход", закроется интернет-магазин и вернет на страницу авторизации

## Тест-кейс №17 — Нажатие кнопки "Удалить", внутри корзины
1. Предшествующие условия:
    - пользователь авторизован
    - открыта главная страница магазина
    - открыта "Корзина"
2. Шаги:
    - навести курсор на кнопку "Удалить" 
    - нажать на кнопку "Удалить" 
3. Ожидаемый результат:
    - при нажатии на кнопку "Удалить", товар будет удален с корзины

## Тест-кейс №18 — Нажатие кнопки "Продолжить ходить по магазину", внутри корзины
1. Предшествующие условия:
    - пользователь авторизован
    - открыта главная страница магазина
    - открыта "Корзина"
2. Шаги:
    - навести курсор на кнопку "Продолжить ходить по магазину" 
    - нажать на кнопку "Продолжить ходить по магазину" 
3. Ожидаемый результат:
    - при нажатии на кнопку "Продолжить ходить по магазину", перейдет обратно в каталог товаров

## Тест-кейс №19 — Нажатие на наименование товара, внутри корзины
1. Предшествующие условия:
    - пользователь авторизован
    - открыта главная страница магазина
    - открыта "Корзина"
2. Шаги:
    - навести курсор на наименование товара 
    - нажать на наименование товара 
3. Ожидаемый результат:
    - при нажатии наименование товара, открывается товар с описанием

## Тест-кейс №20 — Нажатие кнопки "Оформить покупку", внутри корзины
1. Предшествующие условия:
    - пользователь авторизован
    - открыта главная страница магазина
    - открыта "Корзина"
2. Шаги:
    - навести курсор на кнопку "Оформить покупку" 
    - нажать на кнопку "Оформить покупку" 
3. Ожидаемый результат:
    - при нажатии на кнопку "Оформить покупку", открывается новая страница оформления заказа с вводом персональных данных