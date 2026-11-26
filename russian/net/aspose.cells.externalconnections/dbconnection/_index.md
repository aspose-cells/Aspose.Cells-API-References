---
title: "Класс DBConnection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ExternalConnections.DBConnection. Указывает все свойства, связанные с внешним соединением данных ODBC или OLE DB"
type: docs
url: /ru/net/aspose.cells.externalconnections/dbconnection/
---
## DBConnection class

Указывает все свойства, связанные с внешним соединением данных ODBC или OLE DB.

```csharp
public class DBConnection : ExternalConnection
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Указывает, может ли соединение обновляться в фоновом режиме (асинхронно). true, если предпочтительно обновлять соединение асинхронно в фоне; false, если предпочтительно обновлять соединение синхронно на переднем плане. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| override [ClassType](../../aspose.cells.externalconnections/dbconnection/classtype/) { get; } | Получает тип этого объекта [`ExternalConnection`](../externalconnection/). |
| override [Command](../../aspose.cells.externalconnections/dbconnection/command/) { get; set; } | Строка, содержащая команду базы данных, передаваемую API поставщика данных, который будет взаимодействовать с внешним источником для получения данных |
| override [CommandType](../../aspose.cells.externalconnections/dbconnection/commandtype/) { get; set; } | Указывает тип команды OLE DB. 1. Запрос указывает имя куба 2. Запрос указывает SQL‑оператор 3. Запрос указывает имя таблицы 4. Запрос указывает, что предоставлена информация по умолчанию, и интерпретация зависит от поставщика. 5. Запрос направлен к веб‑ориентированному List Data Provider. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Указывает пользовательское описание для этого соединения (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | Получает файл соединения. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Указывает уникальный идентификатор этого соединения. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| [ConnectionInfo](../../aspose.cells.externalconnections/dbconnection/connectioninfo/) { get; set; } | (**Obsolete.**) Строка информации о соединении используется для установления контакта с источником данных OLE DB или ODBC. |
| override [ConnectionString](../../aspose.cells.externalconnections/dbconnection/connectionstring/) { get; set; } | Строка информации о соединении используется для установления контакта с источником данных OLE DB или ODBC. |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Указывает метод аутентификации, используемый при установлении (или повторном установлении) соединения. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Указывает метод аутентификации, используемый при установлении (или повторном установлении) соединения. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Получает идентификатор соединения. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | Указывает, было ли удалено связанное соединение книги. true, если соединение удалено; иначе false. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | True, если соединение ещё не было обновлено впервые; иначе false. Это состояние может возникнуть, когда пользователь сохраняет файл до завершения выполнения запроса. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | True, когда приложение таблицы должно пытаться держать соединение открытым. Когда false, приложение должно закрыть соединение после получения информации. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Указывает имя соединения. Каждое соединение должно иметь уникальное имя. (Наследовано от [`ExternalConnection`](../externalconnection/).) |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Указывает полный путь к внешнему файлу подключения, из которого было создано это подключение. Если подключение не удаётся во время попытки обновить данные и reconnectionMethod=1, приложение таблицы попробует снова, используя информацию из внешнего файла подключения вместо встроенного в книгу объекта подключения. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Указывает, следует ли приложению таблицы всегда и исключительно использовать информацию о подключении во внешнем файле подключения, указанном атрибутом odcFile, при обновлении подключения. Если false, приложение таблицы должно следовать процедуре, указанной атрибутом reconnectionMethod. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | Получает [`ConnectionParameterCollection`](../connectionparametercollection/) для ODBC или веб‑запроса. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| override [PowerQueryFormula](../../aspose.cells.externalconnections/dbconnection/powerqueryformula/) { get; } | Получает определение формулы Power Query. |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) Указывает, что приложение таблицы должно делать, когда подключение не удаётся. Значение по умолчанию — ReConnectionMethodType.Required. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Указывает, что приложение таблицы должно делать, когда подключение не удаётся. Значение по умолчанию — ReConnectionMethodType.Required. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Указывает количество минут между автоматическими обновлениями подключения. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | True, если это подключение должно обновляться при открытии файла; иначе false. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | True, если внешние данные, полученные через подключение для заполнения таблицы, должны сохраняться вместе с книгой; иначе false. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | True, если пароль должен сохраняться как часть строки подключения; иначе False. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| override [SecondCommand](../../aspose.cells.externalconnections/dbconnection/secondcommand/) { get; set; } | Указывает вторую строку команды, которая сохраняется, когда используются полевые элементы PivotTable на основе сервера. Для ODBC‑подключений serverCommand обычно представляет более широкий запрос, чем command (в первом нет предложения WHERE). На основе этих двух команд (Command и ServerCommand) можно заполнить пользовательский интерфейс параметров и построить параметризованные запросы. |
| [SeverCommand](../../aspose.cells.externalconnections/dbconnection/severcommand/) { get; set; } | (**Obsolete.**) Указывает вторую строку команды, которая сохраняется, когда используются полевые элементы PivotTable на основе сервера. Для ODBC‑подключений serverCommand обычно представляет более широкий запрос, чем command (в первом нет предложения WHERE). На основе этих двух команд (Command и ServerCommand) можно заполнить пользовательский интерфейс параметров и построить параметризованные запросы. |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Используется, когда внешний источник данных основан на файле. Когда подключение к такому источнику данных не удаётся, приложение таблицы пытается подключиться напрямую к этому файлу. Может быть указано в виде URI или системно‑специфической нотации пути к файлу. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Получает или задаёт тип DataSource внешнего подключения. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Идентификатор Single Sign On (SSO), используемый для аутентификации между промежуточным сервером spreadsheetML и внешним источником данных. (Inherited from [`ExternalConnection`](../externalconnection/).) |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Obsolete.**) Получает или задаёт тип DataSource внешнего подключения. (Inherited from [`ExternalConnection`](../externalconnection/).) |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassDBConnectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создайте новый экземпляр DBConnection, добавив его в коллекцию
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];

                // Установите базовые свойства
                dbConnection.ConnectionString = "Provider=Microsoft.Jet.OLEDB.4.0;Data Source=C:\\data\\database.mdb;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";

                // Отобразить свойства только для чтения
                Console.WriteLine("DBConnection ClassType: " + dbConnection.ClassType);
                Console.WriteLine("ConnectionString: " + dbConnection.ConnectionString);
                Console.WriteLine("CommandType: " + dbConnection.CommandType);
                Console.WriteLine("Command: " + dbConnection.Command);

                // Сохраните книгу
                workbook.Save("DBConnectionDemo.xlsx");
                Console.WriteLine("DBConnection demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with DBConnection: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [ExternalConnection](../externalconnection/)
* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


