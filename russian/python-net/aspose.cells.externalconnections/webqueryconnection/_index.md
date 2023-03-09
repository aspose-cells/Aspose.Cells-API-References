---
title: WebQueryConnection класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 70
url: /ru/python-net/aspose.cells.externalconnections/webqueryconnection/
is_root: false
---
##  WebQueryConnection класс
 Указывает свойства источника веб-запроса. Веб-запрос извлечет данные из HTML таблиц,
 а также может предоставлять параметры HTTP "Get" для обработки веб-сервером при создании HTML по
включая параметры и элементы параметров.



**Наследование:** [WebQueryConnection](/cells/python-net/aspose.cells.externalconnections/webqueryconnection) → 
[ExternalConnection](/cells/ru/python-net/aspose.cells.externalconnections/externalconnection)



Тип WebQueryConnection предоставляет следующие члены:

###  Характеристики
| Свойство| Описание|
| :- | :- |
| [id](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/id) | Получает идентификатор соединения.|
| [power_query_formula](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/power_query_formula) | Получает определение формулы мощного запроса.|
| [type](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/type) | Получает или задает тип источника данных внешнего подключения.|
| [source_file](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/source_file) | Используется, когда внешний источник данных основан на файлах. При подключении к таким данным<br/> источник не работает, приложение для работы с электронными таблицами пытается напрямую подключиться к этому файлу. Может быть<br/> выраженный в URI или системной нотации пути к файлу.|
| [sso_id](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/sso_id) | Идентификатор для единого входа (SSO), используемый для аутентификации между промежуточным<br/>сервер электронной таблицыML и внешний источник данных.|
| [save_password](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/save_password) |Истинно, если пароль должен быть сохранен как часть строки подключения; в противном случае Ложь.|
| [save_data](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/save_data) | Истинно, если внешние данные, полученные через соединение для заполнения таблицы, должны быть сохранены.<br/> с рабочей тетрадью; в противном случае ложно.|
| [refresh_on_load](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/refresh_on_load) | Истинно, если это соединение должно обновляться при открытии файла; в противном случае ложно.|
| [reconnection_method_type](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/reconnection_method_type) | Указывает, что должно делать приложение для работы с электронными таблицами при сбое подключения.<br/> Значение по умолчанию — ReConnectionMethodType.Required.|
| [reconnection_method](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/reconnection_method) | Указывает, что должно делать приложение для работы с электронными таблицами при сбое подключения.<br/> Значение по умолчанию — ReConnectionMethodType.Required.|
| [only_use_connection_file](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/only_use_connection_file) | Указывает, должно ли приложение для работы с электронными таблицами всегда и только использовать<br/> информация о подключении во внешнем файле подключения, указанном атрибутом odcFile<br/> при обновлении соединения. Если false, то приложение для работы с электронными таблицами<br/> должен следовать процедуре, указанной атрибутом reconnectionMethod|
| [odc_file](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/odc_file) | Указывает полный путь к внешнему файлу подключения, из которого это подключение было<br/> созданный. Если во время попытки обновления данных происходит сбой подключения и reconnectionMethod=1,<br/> затем приложение для работы с электронными таблицами попытается снова использовать информацию из файла внешнего подключения.<br/> вместо объекта подключения, встроенного в книгу.|
| [is_new](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/is_new) | Истинно, если соединение не было обновлено в первый раз; в противном случае ложно.<br/> Это состояние может произойти, когда пользователь сохраняет файл до завершения запроса.|
| [name](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/name) | Задает имя соединения. Каждое соединение должно иметь уникальное имя.|
| [keep_alive](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/keep_alive) | Истинно, когда приложение для работы с электронными таблицами должно прилагать усилия для поддержания соединения.<br/> открыть. При значении false приложение должно закрыть соединение после получения<br/> информация.|
| [refresh_internal](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/refresh_internal) | Указывает количество минут между автоматическими обновлениями соединения.|
| [connection_id](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/connection_id) | Указывает уникальный идентификатор этого соединения.|
| [connection_description](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/connection_description) | Указывает описание пользователя для этого подключения.|
| [is_deleted](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/is_deleted) | Указывает, было ли удалено связанное подключение к книге. верно, если<br/> соединение было удалено; в противном случае ложно.|
| [credentials_method_type](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/credentials_method_type) | Указывает метод проверки подлинности, который будет использоваться при установлении (или повторном установлении) соединения.|
| [credentials](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/credentials) | Указывает метод проверки подлинности, который будет использоваться при установлении (или повторном установлении) соединения.|
| [background_refresh](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/background_refresh) | Указывает, можно ли обновить соединение в фоновом режиме (асинхронно).<br/> Значение true, если предпочтительное использование соединения — асинхронное обновление в фоновом режиме;<br/>false, если предпочтительным использованием соединения является синхронное обновление на переднем плане.|
| [parameters](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/parameters) | Получает [ConnectionParameterCollection](/cells/ru/python-net/aspose.cells.externalconnections/connectionparametercollection) для ODBC или веб-запроса.|
| [is_xml](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/is_xml) | Значение true, если источником веб-запроса является XML (по сравнению с HTML), в противном случае — значение false.|
| [is_xl97](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/is_xl97) | Этот флаг существует для обратной совместимости со старыми существующими файлами электронных таблиц и установлен<br/>значение true, если этот веб-запрос был создан в Microsoft Excel 97.<br/> Это необязательный атрибут, который можно игнорировать.|
| [is_xl2000](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/is_xl2000) | Этот флаг существует для обратной совместимости со старыми существующими файлами электронных таблиц и установлен<br/>значение true, если этот веб-запрос был обновлен в приложении для работы с электронными таблицами более новой версии или равной<br/>до Microsoft Excel 2000.<br/> Это необязательный атрибут, который можно игнорировать.|
| [url](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/url) | URL-адрес для обновления внешних данных.|
| [is_text_dates](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/is_text_dates) | Флаг, указывающий, следует ли импортировать даты в ячейки рабочего листа в виде текста, а не дат.|
| [is_xml_source_data](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/is_xml_source_data) | Флаг, указывающий, что следует импортировать исходные XML-данные вместо самой таблицы HTML.|
| [post](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/post) | Возвращает или задает строку, используемую с почтовым методом ввода данных на веб-сервер.<br/> для возврата данных из веб-запроса.|
| [is_parse_pre](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/is_parse_pre) |Флаг, указывающий, являются ли данные, содержащиеся в тегах PRE HTML на веб-странице,<br/> разбивается на столбцы при импорте страницы в таблицу запросов.|
| [is_html_tables](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/is_html_tables) | Флаг, указывающий, должны ли веб-запросы работать только с таблицами HTML.|
| [html_format](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/html_format) | Как обрабатывать форматирование из источника HTML при переносе данных веб-запроса в<br/> рабочий лист. Актуально, когда sourceData имеет значение True.|
| [is_same_settings](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/is_same_settings) | Флаг, указывающий, следует ли анализировать все таблицы внутри блока PRE с одинаковыми настройками ширины.<br/> как первый ряд.|
| [edit_web_page](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/edit_web_page) | URL-адрес доступной пользователю веб-страницы, отображающей данные веб-запроса. Этот URL сохраняется<br/>в случае, если sourceData="true" и URL-адрес были перенаправлены для ссылки на XML-файл.<br/>Затем пользовательскую страницу можно отобразить в пользовательском интерфейсе и получить XML-данные.<br/> за кулисами.|
| [edit_page](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/edit_page) | URL-адрес доступной пользователю веб-страницы, отображающей данные веб-запроса. Этот URL сохраняется<br/>в случае, если sourceData="true" и URL-адрес были перенаправлены для ссылки на XML-файл.<br/>Затем пользовательскую страницу можно отобразить в пользовательском интерфейсе и получить XML-данные.<br/> за кулисами.|
| [is_consecutive](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection/is_consecutive) | Флаг, указывающий, следует ли рассматривать последовательные разделители как один разделитель.|



###  Смотрите также
* модуль [aspose.cells.externalconnections](..)
* класс [ConnectionParameterCollection](/cells/ru/python-net/aspose.cells.externalconnections/connectionparametercollection)
* класс [ExternalConnection](/cells/ru/python-net/aspose.cells.externalconnections/externalconnection)
* класс [WebQueryConnection](/cells/ru/python-net/aspose.cells.externalconnections/webqueryconnection)
