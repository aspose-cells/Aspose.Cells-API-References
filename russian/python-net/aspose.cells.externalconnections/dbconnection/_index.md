---
title: DBConnection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 30
url: /ru/python-net/aspose.cells.externalconnections/dbconnection/
is_root: false
---
##  DBConnection класс
Задает все свойства, связанные с подключением к внешним данным ODBC или OLE DB.



**Наследование:** [DBConnection](/cells/python-net/aspose.cells.externalconnections/dbconnection) → 
[ExternalConnection](/cells/ru/python-net/aspose.cells.externalconnections/externalconnection)



Тип DBConnection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [id](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/id) | Получает идентификатор соединения.|
| [power_query_formula](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/power_query_formula) | Получает определение формулы мощного запроса.|
| [type](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/type) | Получает или задает тип источника данных внешнего подключения.|
| [source_file](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/source_file) | Используется, когда внешний источник данных основан на файлах.<br/> источник не работает, приложение для работы с электронными таблицами пытается напрямую подключиться к этому файлу.<br/> выраженный в URI или системной нотации пути к файлу.|
| [sso_id](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/sso_id) | Идентификатор для единого входа (SSO), используемый для аутентификации между промежуточным<br/> сервер электронной таблицыML и внешний источник данных.|
| [save_password](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/save_password) | True, если пароль должен быть сохранен как часть строки подключения, в противном случае — False.|
| [save_data](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/save_data) | Истинно, если внешние данные, полученные через соединение для заполнения таблицы, должны быть сохранены.<br/> с рабочей книгой, в противном случае false.|
| [refresh_on_load](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/refresh_on_load) | Истинно, если это соединение должно обновляться при открытии файла;|
| [reconnection_method_type](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/reconnection_method_type) | Указывает, что должно делать приложение для работы с электронными таблицами при сбое подключения.<br/>Значение по умолчанию — ReConnectionMethodType.Required.|
| [reconnection_method](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/reconnection_method) | Указывает, что должно делать приложение для работы с электронными таблицами при сбое подключения.<br/>Значение по умолчанию — ReConnectionMethodType.Required.|
| [only_use_connection_file](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/only_use_connection_file) | Указывает, должно ли приложение для работы с электронными таблицами всегда и только использовать<br/> информация о подключении во внешнем файле подключения, указанном атрибутом odcFile<br/> при обновлении соединения. Если false, то приложение для работы с электронными таблицами<br/> должен следовать процедуре, указанной атрибутом reconnectionMethod|
| [odc_file](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/odc_file) | Указывает полный путь к внешнему файлу подключения, из которого это подключение было<br/> Если во время попытки обновления данных происходит сбой подключения и reconnectionMethod=1,<br/> затем приложение для работы с электронными таблицами попытается снова использовать информацию из файла внешнего подключения.<br/> вместо объекта подключения, встроенного в книгу.|
| [is_new](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/is_new) | Истина, если соединение не обновлялось в первый раз, в противном случае — ложь.<br/> Это состояние может произойти, когда пользователь сохраняет файл до завершения запроса.|
| [name](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/name) | Задает имя соединения.|
| [keep_alive](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/keep_alive) | Истинно, когда приложение для работы с электронными таблицами должно прилагать усилия для поддержания соединения.<br/>Если установлено значение false, приложение должно закрыть соединение после получения<br/> информация.|
| [refresh_internal](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/refresh_internal) | Указывает количество минут между автоматическими обновлениями соединения.|
| [connection_id](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/connection_id) | Указывает уникальный идентификатор этого соединения.|
| [connection_description](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/connection_description) | Указывает описание пользователя для этого соединения.|
| [is_deleted](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/is_deleted) |Указывает, было ли удалено связанное подключение к книге.<br/> в противном случае ложно.|
| [credentials_method_type](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/credentials_method_type) | Указывает метод проверки подлинности, который будет использоваться при установлении (или повторном установлении) соединения.|
| [credentials](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/credentials) | Указывает метод проверки подлинности, который будет использоваться при установлении (или повторном установлении) соединения.|
| [background_refresh](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/background_refresh) | Указывает, можно ли обновить соединение в фоновом режиме (асинхронно).<br/>Значение true, если предпочтительное использование соединения — асинхронное обновление в фоновом режиме;<br/> false, если предпочтительным использованием соединения является синхронное обновление на переднем плане.|
| [parameters](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/parameters) | Получает [ConnectionParameterCollection](/cells/ru/python-net/aspose.cells.externalconnections/connectionparametercollection) для ODBC или веб-запроса.|
| [connection_info](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/connection_info) | Строка информации о подключении используется для связи с источником данных OLE DB или ODBC.|
| [command_type](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/command_type) | Указывает тип команды OLE DB.<br/>1. Запрос указывает имя куба<br/>2. Запрос указывает оператор SQL<br/>3. Запрос указывает имя таблицы<br/>4. Запрос указывает, что была предоставлена информация по умолчанию, а как ее интерпретировать, зависит от провайдера.<br/> 5. Запрос относится к веб-поставщику данных списка.|
| [command](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/command) | Строка, содержащая команду базы данных для передачи поставщику данных API, который<br/> взаимодействовать с внешним источником для получения данных|
| [sever_command](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection/sever_command) |Задает вторую текстовую строку команды, которая сохраняется при использовании сводной таблицы на основе сервера.<br/> поля страницы используются.<br/> Для соединений ODBC serverCommand обычно является более широким запросом, чем команда (не<br/>предложение WHERE присутствует в первом).<br/> Пользовательский интерфейс параметров может быть заполнен, и могут быть созданы параметризованные запросы.|



###  Смотрите также
* модуль [aspose.cells.externalconnections](..)
* класс [ConnectionParameterCollection](/cells/ru/python-net/aspose.cells.externalconnections/connectionparametercollection)
* класс [DBConnection](/cells/ru/python-net/aspose.cells.externalconnections/dbconnection)
* класс [ExternalConnection](/cells/ru/python-net/aspose.cells.externalconnections/externalconnection)
