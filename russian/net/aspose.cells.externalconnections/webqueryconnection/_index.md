---
title: WebQueryConnection
second_title: Справочник по Aspose.Cells для .NET API
description: Указывает свойства источника веб-запроса. Веб-запрос будет извлекать данные из таблиц HTML  а также может предоставлять параметры HTTP Get которые будут обрабатываться веб-сервером при создании HTML с помощью включая параметры и параметр элементы.
type: docs
weight: 3350
url: /ru/net/aspose.cells.externalconnections/webqueryconnection/
---
## WebQueryConnection class

Указывает свойства источника веб-запроса. Веб-запрос будет извлекать данные из таблиц HTML, , а также может предоставлять параметры HTTP "Get", которые будут обрабатываться веб-сервером при создании HTML с помощью включая параметры и параметр элементы.

```csharp
public class WebQueryConnection : ExternalConnection
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh) { get; set; } | Указывает, можно ли обновить соединение в фоновом режиме (асинхронно). true, если предпочтительным использованием соединения является асинхронное обновление в фоновом режиме; false, если предпочтительным использованием соединения является синхронное обновление на переднем плане. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription) { get; set; } | Указывает описание пользователя для этого соединения |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid) { get; } | Уникальный идентификатор этого соединения. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype) { get; set; } | Указывает метод аутентификации, который будет использоваться при установлении (или повторном установлении) соединения. |
| [EditWebPage](../../aspose.cells.externalconnections/webqueryconnection/editwebpage) { get; set; } | URL-адрес доступной пользователю веб-страницы, отображающей данные веб-запроса. Этот URL-адрес сохраняется в случае, если sourceData="true" и URL-адрес был перенаправлен для ссылки на XML-файл. Затем пользовательская страница может отображаться в пользовательском интерфейсе, а XML-данные могут быть извлечены за кулисами. |
| [HtmlFormat](../../aspose.cells.externalconnections/webqueryconnection/htmlformat) { get; set; } | Как обрабатывать форматирование из источника HTML при переносе данных веб-запроса на рабочий лист . Актуально, когда sourceData имеет значение True. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id) { get; } | Получает идентификатор соединения. |
| [IsConsecutive](../../aspose.cells.externalconnections/webqueryconnection/isconsecutive) { get; set; } | Флаг, указывающий, следует ли рассматривать последовательные разделители как один разделитель. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted) { get; set; } | Указывает, было ли удалено связанное подключение к книге. true, если соединение было удалено; в противном случае ложно. |
| [IsHtmlTables](../../aspose.cells.externalconnections/webqueryconnection/ishtmltables) { get; set; } | Флаг, указывающий, должны ли веб-запросы работать только с таблицами HTML. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew) { get; set; } | Истинно, если соединение не обновлялось в первый раз; в противном случае ложно. Это состояние может произойти, когда пользователь сохраняет файл до завершения запроса. |
| [IsParsePre](../../aspose.cells.externalconnections/webqueryconnection/isparsepre) { get; set; } | Флаг, указывающий, разбиваются ли данные, содержащиеся в тегах HTML PRE на веб-странице на столбцы при импорте страницы в таблицу запросов. |
| [IsSameSettings](../../aspose.cells.externalconnections/webqueryconnection/issamesettings) { get; set; } | Флаг, указывающий, следует ли анализировать все таблицы внутри блока PRE с теми же настройками ширины , что и первая строка. |
| [IsTextDates](../../aspose.cells.externalconnections/webqueryconnection/istextdates) { get; set; } | Флаг, указывающий, следует ли импортировать даты в ячейки рабочего листа в виде текста, а не дат. |
| [IsXl2000](../../aspose.cells.externalconnections/webqueryconnection/isxl2000) { get; set; } | Этот флаг существует для обратной совместимости с более старыми существующими файлами электронных таблиц и устанавливается в true, если этот веб-запрос был обновлен в приложении для работы с электронными таблицами более новой версии. чем или равно Microsoft Excel 2000. Это необязательный атрибут, который можно игнорировать. |
| [IsXl97](../../aspose.cells.externalconnections/webqueryconnection/isxl97) { get; set; } | Этот флаг существует для обратной совместимости со старыми существующими файлами электронных таблиц и устанавливается в true, если этот веб-запрос был создан в Microsoft Excel 97. Это необязательный атрибут, который можно игнорировать. |
| [IsXml](../../aspose.cells.externalconnections/webqueryconnection/isxml) { get; set; } | true, если источником веб-запроса является XML (а не HTML), в противном случае false. |
| [IsXmlSourceData](../../aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata) { get; set; } | Флаг, указывающий, что исходные данные XML должны быть импортированы вместо самой таблицы HTML. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive) { get; set; } | Истинно, когда приложение электронных таблиц должно прилагать усилия, чтобы поддерживать соединение открытым. При значении false приложение должно закрыть соединение после получения информации . |
| [Name](../../aspose.cells.externalconnections/externalconnection/name) { get; set; } | Указывает имя подключения. Каждое соединение должно иметь уникальное имя. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile) { get; set; } | Указывает полный путь к файлу внешнего подключения, из которого было создано это подключение . Если во время попытки обновления данных происходит сбой соединения, а reconnectionMethod=1, , то приложение для работы с электронными таблицами попытается повторить попытку, используя информацию из внешнего файла соединения вместо встроенного объекта соединения. внутри рабочей тетради. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile) { get; set; } | Указывает, должно ли приложение электронных таблиц всегда и только использовать информацию о соединении во внешнем файле соединения, указанном атрибутом odcFile при обновлении соединения. Если false, то приложение электронной таблицы должно следовать процедуре, указанной атрибутом reconnectionMethod |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters) { get; } | Получает[`ConnectionParameterCollection`](../connectionparametercollection)для ODBC или веб-запроса. |
| [Post](../../aspose.cells.externalconnections/webqueryconnection/post) { get; set; } | Возвращает или задает строку, используемую с почтовым методом ввода данных на веб-сервер для возврата данных из веб-запроса. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula) { get; } | Получает определение формулы мощного запроса. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype) { get; set; } | Указывает, что должно делать приложение для работы с электронными таблицами при сбое соединения. Значение по умолчанию — ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal) { get; set; } | Указывает количество минут между автоматическим обновлением соединения. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload) { get; set; } | True, если это соединение должно обновляться при открытии файла; в противном случае ложно. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata) { get; set; } | Истинно, если внешние данные, полученные через соединение для заполнения таблицы, должны быть сохранены вместе с рабочей книгой; в противном случае ложно. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword) { get; set; } | True, если пароль должен быть сохранен как часть строки подключения; в противном случае Ложь. |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile) { get; set; } | Используется, когда внешний источник данных основан на файлах. Когда подключение к такому источнику данных не удается, приложение для работы с электронными таблицами пытается напрямую подключиться к этому файлу. Может быть выраженным в URI или системной нотации пути к файлу. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid) { get; set; } | Идентификатор для единого входа (SSO), используемый для аутентификации между промежуточным сервером электронной таблицы ML и внешним источником данных. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type) { get; set; } | Получает или задает тип источника данных внешнего подключения. |
| [Url](../../aspose.cells.externalconnections/webqueryconnection/url) { get; set; } | URL для обновления внешних данных. |

### Смотрите также

* class [ExternalConnection](../externalconnection)
* пространство имен [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
