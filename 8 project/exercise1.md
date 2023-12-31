**Горячие клавиши, которыми можно открыть Chrome DevTools**

- Ctrl+U (при русской раскладке – буква «Г») – для просмотра кода страница («View page code»). Чтобы внести изменения, кликаем на кнопку «Править».
- Ctrl+Shift+J («О») – для открытия консоли Java («JavaScript console»). Инструменты открываются после нажатия на вкладку «Console».
- Ctrl+Shift+I (Ш) – чтобы выбрать инструменты разработчика («Developer tools»).
- Ctrl+Shift+C - чтобы выбрать определенный элемент, нажмите на значок селектора элемента или воспользоваться клавиатурной комбинацией.
- Есть и универсальная горячая клавиша — F12. Она запускает консоль почти во всех веб-обозревателях.

**Возможности, которые предоставляет Chrome DevTools:**

1. **Панель Elements**

Используется для выбора и редактирования любых HTML элементов на странице. Позволяет свободно манипулировать DOM и CSS.

Вкладка содержит две кнопки: Выбор элемента с помощью курсора и Переключение в режим выбора устройств, она пригодится при разработке адаптивных интерфейсов, мобильных версий сайтов или для тестирования страниц с разным разрешением монитора. При выборе любого DOM элемента на вкладке Styles будет отображаться все CSS правила применяемые к нему, в том числе и неактивные. Все правила разбиты на блоки и упорядочены по убыванию специфичности селектора. Можно на лету менять значения, деактивировать и дописывать новые правила и смотреть как это влияет на отображение. Также для выбранного элемента DOM доступно еще несколько вкладок: Event Listeners — содержит все события относящиеся к данному элементу, DOM Breakpoints — точки останова для элемента и Properties — список всех свойств для элемента. Также могут быть дополнительные вкладки добавляемые расширениями для Chrome.

Ключевые возможности:

-Просмотр и редактирование в лайв режиме любого элемента DOM.

-Просмотр и изменение CSS правил применяемых к любому выбранному элементу в панели Styles.

-Просмотр всего списка событий и свойств для элемента на соответствующих вкладках.

2. **Панель Console**

Необходима для логирования диагностической информации в процессе разработки или взаимодействие с JavaScript на странице. Также все ошибки в JavaScript коде, будут выводится здесь с указанием файла и конкретного места в нем где произошла ошибка. Так же в консоль можно выводить XHR запросы. Есть возможность сохранять логи в отдельный файл.

Консоль содержит ряд инструментов и настроек для фильтрации выводимых сообщений, очистки консоли и запрета очистки логов при перезагрузке страницы — Preserve log.

Также консоль может отобразить/скрыть в виде отдельной вкладки находясь на любой другой вкладке и не покидая ее нажав клавишу Esc.

**Ключевые возможности:**

- Использование консоли как отдельной панели или как окна рядом с любой другой панелью.
- Возможность группировать большое колличество сообщения или выведите их на отдельных строках.
- Очистка всех логов или сохранения их между перезагрузкой страниц, сохранение логов в отдельный файл.
- Фильтрация по типу сообщения или по регулярному выражению.
- Логирование XHR запросов.

3. **Панель Sources**

Инструмент Sources представляет собой своего рода IDE, где мы можем посмотреть все файлы подключенные на нашей странице. Мы можем посмотреть их содержимое, отредактировать код, скопировать его или сохранить измененный файл, как новый файл. Данную вкладку можно использовать и как полноценный редактор кода подключаясь к локальным файлам через Workspaces.

Также Sources используется для отладки JavaScript используя брейкпоинты. Для работы с брейкпоинтами предусмотрено большое количество специальных кнопок и доп. возможностей о которых больше можно узнать в официальной документации.

**Ключевые возможности:**

- Отладка Вашего кода с помощью брейкпоинтов.
- Использование браузера в качестве IDE с помощью Workspaces.
- Запуск сниппетов с любой страницы.

4. **Панель Network**

Позволяет мониторить процесс загрузки страницы и всех файлов которые подгружаются при загрузке. Ее удобно использовать для оптимизация загрузки страниц и мониторинг запросов. На панели отображается таблица всех запросов к данным и файлам, над ней располагаются кнопки для фильтрации нужных Вам запросов, очистки таблицы или включения/отключения записи запросов, кнопки управления отображением таблицы. Также есть дополнительные переключатели: Preserve log — не очищать таблицу при перезагрузке страницы, Disable cache — отключить кэш браузера (будет работать только при открытом Dev Tools), Offline — эмулирует отсутствие интернета, также соседний переключатель позволяющий эмулировать скорость скачивания/загрузки данных и ping для различных типов сетей.

Под таблицей указано количество всех запросов, общее количество загруженных данных, общее время загрузки всех данных, время загрузки и построения DOM дерева и время загрузки всех ресурсов влияющих на отображение этой страницы.

**Ключевые возможности:**

- Возможность отключить кэширование или установление ограничения пропускной способности.
- Получение подробной таблицы с информацией о каждом запросе.
- Фильтрация и поиск по всему списку запросов.

5. **Панель Performance**

Панель отображает таймлайн использования сети, выполнения JavaScript кода и загрузки памяти. После первоначального построения графиков таймлайн, будут доступны подробные данные о выполнение кода и всем жизненном цикле страницы. Будет возможно ознакомится с временем исполнения отдельных частей кода, появится возможность выбрать отдельный промежуток на временной шкале и ознакомится с тем какие процессы происходили в этот момент.

Инструмент применяется для улучшение производительности работы Вашей страницы в целом.

**Ключевые возможности:**

- Возможность сделать запись чтобы проанализировать каждое событие, которое произошло после загрузки страницы или взаимодействия с пользователем.
- Возможность просмотреть FPS, загрузку CPU и сетевые запросы в области Overview.
- Щелкните по событию в диаграмме, чтобы посмотреть детали об этом.
- Возможность изменить масштаб таймлайн, чтобы сделать анализ проще.

6. **Панель Memory и JavaScript Profiler**

Содержит несколько различных профайлеров для отслеживания нагрузки которую оказывает выполнение кода на систему:

JavaScript CPU Profiler (был вынесен в отдельную панель JavaScript Profiler ) — позволяет узнать сколько процессорного времени занимает выполнение различных частей вашего JS кода. Take Heap Snapshot — показывает распределение памяти среди JS объектов и связанные с ним элементы DOM.

Record Allocation Timeline — записывает и отображает распределение памяти между переменными в коде. Эффективен для устранения утечек памяти.

Record Allocation Profile — записывает и отображает распределение памяти на выполнение отдельных JS функций.

**Ключевые возможности:**

- Исправление проблем с памятью.
- Профилирование CPU при работе с JavaScript.

7. **Панель Application**

Вкладка для инспектирования и очистки всех загруженных ресурсов, включая IndexedDB или Web SQL базы данных, local и session storage, куков, кэша приложения, изображений, шрифтов и таблиц стилей.

**Ключевые возможности:**

- Быстрая очистка хранилищ и кэша.
- Инспектирование и управление хранилищами, базами данных и кэшем.
- Инспектирование и удаление файлов cookie.

8. **Панель Security**

На вкладке можно ознакомится с протоколом безопасности при его наличии и просмотреть данные о сертификате безопасности, если он есть.

Инструмент используется для отладки проблем смешанного контента, проблем сертификатов и прочее.

**Ключевые возможности:**

- Окно Security Overview быстро подскажет безопасна ли текущая страница или нет.
- Возможность просмотреть отдельные источники, чтобы просмотреть соединение и детали сертификата (для безопасных источников) или узнать, какие запросы не защищены (для небезопасных источников).

9. **Панель Audits**

После выбора нужных настроек и нажатия кнопки Run панель аудита анализирует как загружается страница и затем предоставляет предложения по оптимизации для уменьшения времени загрузки страницы и увеличению ее отзывчивости.

Анализируются такие параметры как: кэширование ресурсов, gzip сжатие, наличие неиспользуемых частей JS кода и CSS правил и много других параметров. Далее пользователю выводится сгруппированных список рекомендаций за счет выполнения которых можно существенно оптимизировать скорость загрузки и отзывчивости страницы.

10. **Lighthouse**

Автоматизированный инструмент с открытым исходным кодом для улучшения качества прогрессивных веб-приложений.устраняет большую часть ручного тестирования, которое требовалось ранее. Вы даже можете использовать Lighthouse в системах непрерывной интеграции для выявления регрессий. Lighthouse — это автоматизированный инструмент с открытым исходным кодом для улучшения качества веб-страниц. Вы можете запустить его на любой веб-странице, общедоступной или требующей аутентификации. У него есть аудиты производительности, доступности, прогрессивных веб-приложений, SEO и многого другого.

Lighthouse оценивает классические сайты по четырём критериям: производительность, лучшие практики, SEO и доступность. Для сайтов, выполненных по технологии PWA (прогрессивные веб-приложения), добавляется пятый критерий — progressive web app. Как использовать Lighthouse

Чтобы запустить проверку, перейдите во вкладку Lighthouse и нажмите на кнопку Generate report. Во время тестирования инструмент будет менять размеры браузера, имитировать отключение и подключение интернета и выполнять другие операции. В конце вы получите оценки качества сайта по 100-балльной шкале: чем выше оценка, тем лучше. При этом на чистоту проверки могут влиять разные факторы, в том числе интернет-соединение и расширения Chrome. Поэтому лучше запускать тест в режиме инкогнито, закрыв остальные вкладки.

**Посмотреть, как выглядит страница с телефона и планшета** При создании адаптивных сайтов или веб-приложений полезно знать, как выглядит страница на планшете и мобильных устройствах. С помощью инструментов разработчика вы можете сделать это за несколько секунд. Для этого откройте Chrome Devtools, а затем кликните на иконку Toggle device toolbar в левом углу или нажмите комбинацию Ctrl+Shift+M. Над страницей появится панель с режимами эмуляции из мобильных устройств и планшетов. По умолчанию панель инструментов открывается в режиме адаптивного окна просмотра. Чтобы изменить область до нужных размеров, задайте ширину или потяните за границы рабочей области. А если хотите увидеть, как страница отображается на конкретных устройствах, например, на iPhone 5, кликните на Responsive и выберите подходящий девайс.

**Запускаем Web Inspector**

Есть несколько способов открыть Web Inspector:

- Ctrl + SHIFT + I — Открывает панель элементов.
- Ctrl + SHIFT + J или F12 — Открывает консоль
- Ctrl + SHIFT + C — Позволяет выбрать элемент, с помощью мыши, в самом документе и открыть его во вкладке «Elements» Можно нажать на любом элементе на странице правой кнопкой мыши и выбрать «Inspect Element (Просмотр кода элемента)». Можно открыть Web Inspector из меню: Иконка с ключом -> Инструменты -> Инструменты разработчика (Tools -> Developer tools)
