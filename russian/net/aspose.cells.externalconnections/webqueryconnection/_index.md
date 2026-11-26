---
title: "Класс WebQueryConnection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.ExternalConnections.WebQueryConnection class. Указывает свойства источника веб‑запроса. Веб‑запрос будет извлекать данные из HTML‑таблиц и также может передавать параметры HTTP GET, которые обрабатываются веб‑сервером при генерации HTML, включая параметры и элементы параметров."
type: docs
url: /ru/net/aspose.cells.externalconnections/webqueryconnection/
---
## WebQueryConnection class

Указывает свойства источника веб‑запроса. Веб‑запрос получает данные из HTML‑таблиц и может также передавать параметры HTTP "Get", которые обрабатываются веб‑сервером при генерации HTML, включая параметры и элементы параметров.

```csharp
public class WebQueryConnection : ExternalConnection
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Указывает, может ли соединение обновляться в фоновом режиме (асинхронно). true, если предпочтительно обновлять соединение асинхронно в фоне; false, если предпочтительно обновлять соединение синхронно на переднем плане. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/webqueryconnection/classtype/) { get; } | Получает тип этого объекта [`ExternalConnection`](../externalconnection/). |
| virtual [Command](../../aspose.cells.externalconnections/externalconnection/command/) { get; set; } | Строка, содержащая команду базы данных, которую следует передать API поставщика данных, который будет взаимодействовать с внешним источником для получения данных (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| virtual [CommandType](../../aspose.cells.externalconnections/externalconnection/commandtype/) { get; set; } | Указывает тип команды OLE DB. 1. Запрос указывает имя куба 2. Запрос указывает оператор SQL 3. Запрос указывает имя таблицы 4. Запрос указывает, что предоставлена информация по умолчанию, и как её интерпретировать, зависит от провайдера. 5. Запрос направлен к веб‑основному поставщику данных списка. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Указывает пользовательское описание для этого соединения (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| override [ConnectionFile](../../aspose.cells.externalconnections/webqueryconnection/connectionfile/) { get; } | Получает файл соединения. |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Указывает уникальный идентификатор этого соединения. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionString](../../aspose.cells.externalconnections/externalconnection/connectionstring/) { get; set; } | Строка информации о соединении используется для установления контакта с источником данных OLE DB или ODBC. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Указывает метод аутентификации, используемый при установлении (или повторном установлении) соединения. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Указывает метод аутентификации, используемый при установлении (или повторном установлении) соединения. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| [EditPage](../../aspose.cells.externalconnections/webqueryconnection/editpage/) { get; set; } | (**Obsolete.**) URL пользовательской веб‑страницы, отображающей данные веб‑запроса. Этот URL сохраняется в случае, когда sourceData="true" и url был перенаправлен к XML‑файлу. Затем пользовательская страница может быть показана в интерфейсе, а XML‑данные могут быть получены в фоновом режиме. |
| [EditWebPage](../../aspose.cells.externalconnections/webqueryconnection/editwebpage/) { get; set; } | URL пользовательской веб‑страницы, отображающей данные веб‑запроса. Этот URL сохраняется в случае, когда sourceData="true" и url был перенаправлен к XML‑файлу. Затем пользовательская страница может быть показана в интерфейсе, а XML‑данные могут быть получены в фоновом режиме. |
| [HtmlFormat](../../aspose.cells.externalconnections/webqueryconnection/htmlformat/) { get; set; } | Как обрабатывать форматирование из HTML‑источника при импорте данных веб‑запроса в лист. Актуально, когда sourceData равно True. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Получает идентификатор соединения. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| [IsConsecutive](../../aspose.cells.externalconnections/webqueryconnection/isconsecutive/) { get; set; } | Флаг, указывающий, следует ли рассматривать последовательные разделители как один разделитель. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | Указывает, было ли удалено связанное соединение книги. true, если соединение удалено; иначе false. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| [IsHtmlTables](../../aspose.cells.externalconnections/webqueryconnection/ishtmltables/) { get; set; } | Флаг, указывающий, должны ли веб‑запросы работать только с HTML‑таблицами. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | True, если соединение ещё не было обновлено впервые; иначе false. Это состояние может возникнуть, когда пользователь сохраняет файл до завершения выполнения запроса. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| [IsParsePre](../../aspose.cells.externalconnections/webqueryconnection/isparsepre/) { get; set; } | Флаг, указывающий, разбираются ли данные, содержащиеся внутри тегов HTML PRE на веб‑странице, в столбцы при импорте страницы в таблицу запросов. |
| [IsSameSettings](../../aspose.cells.externalconnections/webqueryconnection/issamesettings/) { get; set; } | Флаг, указывающий, следует ли разбирать все таблицы внутри блока PRE с теми же настройками ширины, что и первая строка. |
| [IsTextDates](../../aspose.cells.externalconnections/webqueryconnection/istextdates/) { get; set; } | Флаг, указывающий, следует ли импортировать даты в ячейки листа как текст, а не как даты. |
| [IsXl2000](../../aspose.cells.externalconnections/webqueryconnection/isxl2000/) { get; set; } | Этот флаг существует для обеспечения обратной совместимости со старыми существующими файлами электронных таблиц и устанавливается в true, если этот веб‑запрос был обновлён в приложении электронных таблиц, версии не ниже Microsoft Excel 2000. Это необязательный атрибут, который можно игнорировать. |
| [IsXl97](../../aspose.cells.externalconnections/webqueryconnection/isxl97/) { get; set; } | Этот флаг существует для обеспечения обратной совместимости со старыми существующими файлами электронных таблиц и устанавливается в true, если этот веб‑запрос был создан в Microsoft Excel 97. Это необязательный атрибут, который можно игнорировать. |
| [IsXml](../../aspose.cells.externalconnections/webqueryconnection/isxml/) { get; set; } | true, если источник веб‑запроса — XML (в отличие от HTML), иначе false. |
| [IsXmlSourceData](../../aspose.cells.externalconnections/webqueryconnection/isxmlsourcedata/) { get; set; } | Флаг, указывающий, что данные источника XML должны быть импортированы вместо самой HTML‑таблицы. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | True, когда приложение таблицы должно пытаться держать соединение открытым. Когда false, приложение должно закрыть соединение после получения информации. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Указывает имя соединения. Каждое соединение должно иметь уникальное имя. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Указывает полный путь к внешнему файлу подключения, из которого было создано это подключение. Если подключение не удаётся во время попытки обновить данные и reconnectionMethod=1, приложение таблицы попробует снова, используя информацию из внешнего файла подключения вместо встроенного в книгу объекта подключения. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Указывает, следует ли приложению таблицы всегда и исключительно использовать информацию о подключении во внешнем файле подключения, указанном атрибутом odcFile, при обновлении подключения. Если false, приложение таблицы должно следовать процедуре, указанной атрибутом reconnectionMethod. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | Получает [`ConnectionParameterCollection`](../connectionparametercollection/) для ODBC или веб‑запроса. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Post](../../aspose.cells.externalconnections/webqueryconnection/post/) { get; set; } | Возвращает или задаёт строку, используемую методом POST для ввода данных на веб‑сервер и получения данных из веб‑запроса. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula/) { get; } | Получает определение формулы Power Query. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) Указывает, что приложение таблицы должно делать, когда подключение не удаётся. Значение по умолчанию — ReConnectionMethodType.Required. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Указывает, что приложение таблицы должно делать, когда подключение не удаётся. Значение по умолчанию — ReConnectionMethodType.Required. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Указывает количество минут между автоматическими обновлениями подключения. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | True, если это подключение должно обновляться при открытии файла; иначе false. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | True, если внешние данные, полученные через подключение для заполнения таблицы, должны сохраняться вместе с книгой; иначе false. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | True, если пароль должен сохраняться как часть строки подключения; иначе False. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| virtual [SecondCommand](../../aspose.cells.externalconnections/externalconnection/secondcommand/) { get; set; } | Указывает вторую строку текста команды, которая сохраняется, когда используются полевые элементы PivotTable на основе сервера. Для ODBC‑соединений serverCommand обычно представляет более широкий запрос, чем command (в первом отсутствует условие WHERE). На основе этих двух команд (Command и ServerCommand) пользовательский интерфейс параметров может быть заполнен, а параметризованные запросы могут быть построены (наследовано от [`ExternalConnection`](../externalconnection/)). |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Используется, когда внешний источник данных основан на файле. Когда подключение к такому источнику данных не удаётся, приложение таблицы пытается подключиться напрямую к этому файлу. Может быть указано в виде URI или системно‑специфической нотации пути к файлу. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Получает или задаёт тип DataSource внешнего подключения. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Идентификатор Single Sign On (SSO), используемый для аутентификации между промежуточным сервером spreadsheetML и внешним источником данных. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsolete.**) Получает или задаёт тип DataSource внешнего подключения. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Url](../../aspose.cells.externalconnections/webqueryconnection/url/) { get; set; } | URL, используемый для обновления внешних данных. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassWebQueryConnectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();

            try
            {
                // Создать соединение веб‑запроса через коллекцию
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];
                
                connection.Url = "https://example.com/financial-data";
                connection.IsHtmlTables = true;
                connection.IsTextDates = true;
                connection.HtmlFormat = HtmlFormatHandlingType.All;

                Console.WriteLine($"Web query URL: {connection.Url}");
                Console.WriteLine($"HTML tables only: {connection.IsHtmlTables}");

                workbook.Save("WebQueryConnectionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with WebQueryConnection: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


