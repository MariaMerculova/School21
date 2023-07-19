## Коды ответов

**2xx — успешно**
Эти коды состояния HTTP указывают на успешное принятие сервером клиентского запроса.

В IIS 7.0 или более поздних версий используются перечисленные ниже коды состояния успеха HTTP.

Код	Описание	Примечания  
**200**	- OK -	Клиентский запрос успешно обработан.  
**201**	- Создано -	Клиентский запрос был выполнен и привел к созданию одного или нескольких новых ресурсов.  
**202**	- Accepted -	Клиентский запрос принят к обработке, но обработка еще не завершена.  
**203**	- Недостоверные сведения -	Клиентский запрос выполнен успешно, но вложенное содержимое было изменено по сравнению с ответом исходного сервера.  
**204**	- Содержимое отсутствует -	Сервер успешно выполнил запрос и в содержимом ответа нет дополнительного содержимого для отправки.  
**205**	- Сброс содержимого -	Сервер выполнил запрос и хочет, чтобы агент пользователя сбросил представление документов, в результате которого запрос был отправлен, в исходное состояние, полученное от исходного сервера.  
**206**	- Неполное содержимое -	Сервер успешно выполняет запрос диапазона для целевого ресурса путем передачи одной или нескольких частей выбранного представления.  

**4xx — ошибка клиента**  
Эти коды состояния HTTP указывают на возникновение ошибки, вероятно, на стороне клиентского браузера. Например, клиентский браузер мог запросить несуществующую страницу. Или не предоставить достоверные сведения для проверки подлинности.

В IIS 7.0 или более поздних версий используются перечисленные ниже коды состояния клиентской ошибки HTTP.

Код	Описание	Примечания  
**400** -	Недопустимый запрос -	Серверу не удалось распознать запрос из-за ошибки в синтаксисе. Клиенту не следует повторять запрос без внесения изменений. Дополнительные сведения см. в разделе Устранение ошибок HTTP 400 в IIS.  
**401** -	Отказано в доступе -	Запрос не был применен, так как в нем отсутствуют действительные учетные данные для проверки подлинности для целевого ресурса.  
**403** -	Запрещено -	Сервер распознал запрос, но отказывается его выполнить.  
**404** -	Не найдено -	Исходный сервер не нашел текущее представление целевого ресурса или не хочет раскрывать, что он существует.  
**405** -	Метод запрещен -	Метод, полученный в строке запроса, известен исходному серверу, но не поддерживается целевым ресурсом.  
**406** -	Браузер клиента не принимается тип MIME запрашиваемой страницы.	  
**408** -	Истекло время ожидания запроса -	Сервер не получил сообщение о завершении запроса в течение времени, когда он был готов к ожиданию.  
**412** -	Необходимое условие не выполнено -	Одно или несколько условий, заданных в полях заголовка запроса, при тестировании на сервере оцениваются как false.  

**5xx — ошибка сервера**  
Эти коды состояния HTTP 5xx указывают на невозможность выполнения сервером запроса из-за того, что сервер сталкивается с ошибкой.  

В IIS более поздних версий используются нижеприведенные коды состояния ошибки сервера HTTP.  

Код	Описание	Примечания  
**500**	- Внутренняя ошибка сервера -	Сервер обнаружил неожиданное условие, препятствующее выполнению запроса  
**501**	- Значения, указанные в заголовке, определяют нереализованную конфигурацию -	Сервер не поддерживает функциональные возможности, необходимые для выполнения данного запроса  
**502**	- Веб-сервером в качестве шлюза или прокси-сервера получен недопустимый ответ -	Сервер, выступая в качестве шлюза или прокси-сервера, получил недопустимый ответ от входящего сервера, к которому он обращался при попытке выполнить запрос. Для получения дополнительной информации см. раздел Устранение ошибок 502 в ARR.  
**503** -	Служба недоступна -	Сервер сейчас не может обработать запрос из-за временной перегрузки или запланированного обслуживания. Вероятно, после некоторой задержки проблема будет устранена.  

**Код ответа: 200. Тело ответа:**  
```
    {
        "name": "Малышева Екатерина Матвеевна",
        "birthday": "1995-06-01",
        "post": "Бухгалтер"
    },
    {
        "name": "Капустин Роман Артёмович",
        "birthday": "1991-01-18",
        "post": "Финансовый аналитик"
    },
    {
        "name": "Касьянов Ярослав Ярославович",
        "birthday": "1989-07-29",
        "post": "Кредитный эксперт"
    },
    {
        "name": "Белова Елизавета Руслановна",
        "birthday": "1997-04-13",
        "post": "Аудитор"
    },
    {
        "name": "Романов Константин Александрович",
        "birthday": "2001-12-14",
        "post": "Кассир"
    },
```

**Код ответа: 401. Тело ответа:**
```
{
  "message": "Неверные данные для авторизации."
}
```
**Код ответа: 400. Тело ответа:**
```
{
  "message": "Неверно составлен запрос."
}
```