---
title: "Класс ExternalConnection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.ExternalConnections.ExternalConnection class. Указывает внешнее соединение данных"
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/
---
## ExternalConnection class

Указывает внешнее соединение данных

```csharp
public abstract class ExternalConnection
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh/) { get; set; } | Указывает, может ли соединение обновляться в фоновом режиме (асинхронно). true, если предпочтительно обновлять соединение асинхронно в фоне; false, если предпочтительно обновлять соединение синхронно в переднем плане. |
| abstract [ClassType](../../aspose.cells.externalconnections/externalconnection/classtype/) { get; } | Получает тип этого объекта `ExternalConnection`. |
| virtual [Command](../../aspose.cells.externalconnections/externalconnection/command/) { get; set; } | Строка, содержащая команду базы данных, передаваемую API поставщика данных, который будет взаимодействовать с внешним источником для получения данных |
| virtual [CommandType](../../aspose.cells.externalconnections/externalconnection/commandtype/) { get; set; } | Указывает тип команды OLE DB. 1. Запрос указывает имя куба 2. Запрос указывает SQL‑оператор 3. Запрос указывает имя таблицы 4. Запрос указывает, что предоставлена информация по умолчанию, и интерпретация зависит от поставщика. 5. Запрос направлен к веб‑ориентированному List Data Provider. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription/) { get; set; } | Указывает пользовательское описание для этого соединения |
| virtual [ConnectionFile](../../aspose.cells.externalconnections/externalconnection/connectionfile/) { get; } | Получает файл соединения. |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid/) { get; } | (**Obsolete.**) Указывает уникальный идентификатор этого соединения. |
| virtual [ConnectionString](../../aspose.cells.externalconnections/externalconnection/connectionstring/) { get; set; } | Строка информации о соединении используется для установления контакта с источником данных OLE DB или ODBC. |
| [Credentials](../../aspose.cells.externalconnections/externalconnection/credentials/) { get; set; } | (**Obsolete.**) Указывает метод аутентификации, используемый при установлении (или повторном установлении) соединения. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype/) { get; set; } | Указывает метод аутентификации, используемый при установлении (или повторном установлении) соединения. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id/) { get; } | Получает идентификатор соединения. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted/) { get; set; } | Указывает, было ли удалено связанное соединение книги. true, если соединение удалено; иначе false. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew/) { get; set; } | True, если соединение ещё не было обновлено впервые; иначе false. Такое состояние может возникнуть, когда пользователь сохраняет файл до завершения выполнения запроса. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive/) { get; set; } | True, когда приложение электронных таблиц должно стараться держать соединение открытым. При false приложение должно закрыть соединение после получения информации. |
| [Name](../../aspose.cells.externalconnections/externalconnection/name/) { get; set; } | Указывает имя соединения. Каждое соединение должно иметь уникальное имя. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile/) { get; set; } | Указывает полный путь к файлу внешнего соединения, из которого было создано данное соединение. Если соединение не удаётся во время попытки обновления данных, и reconnectionMethod=1, то приложение электронных таблиц попробует снова, используя информацию из файла внешнего соединения вместо объекта соединения, встроенного в книгу. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/) { get; set; } | Указывает, должно ли приложение электронных таблиц всегда и исключительно использовать информацию о соединении из внешнего файла соединения, указанного атрибутом odcFile, при обновлении соединения. Если false, то приложение должно следовать процедуре, указанной атрибутом reconnectionMethod. |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters/) { get; } | Получает [`ConnectionParameterCollection`](../connectionparametercollection/) для ODBC или веб‑запроса. |
| virtual [PowerQueryFormula](../../aspose.cells.externalconnections/externalconnection/powerqueryformula/) { get; } | Получает определение формулы Power Query. |
| [ReconnectionMethod](../../aspose.cells.externalconnections/externalconnection/reconnectionmethod/) { get; set; } | (**Obsolete.**) Указывает, что должно делать приложение электронных таблиц при сбое соединения. Значение по умолчанию — ReConnectionMethodType.Required. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/) { get; set; } | Указывает, что должно делать приложение электронных таблиц при сбое соединения. Значение по умолчанию — ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal/) { get; set; } | Указывает количество минут между автоматическими обновлениями соединения. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload/) { get; set; } | True, если это соединение должно обновляться при открытии файла; иначе — false. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata/) { get; set; } | True, если внешние данные, полученные через соединение для заполнения таблицы, должны сохраняться вместе с книгой; иначе — false. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword/) { get; set; } | True, если пароль должен сохраняться как часть строки соединения; иначе — False. |
| virtual [SecondCommand](../../aspose.cells.externalconnections/externalconnection/secondcommand/) { get; set; } | Указывает вторую строку команды, которая сохраняется, когда используются полевые элементы PivotTable на основе сервера. Для ODBC‑подключений serverCommand обычно представляет более широкий запрос, чем command (в первом нет предложения WHERE). На основе этих двух команд (Command и ServerCommand) можно заполнить пользовательский интерфейс параметров и построить параметризованные запросы. |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile/) { get; set; } | Используется, когда внешний источник данных основан на файле. Когда соединение с таким источником данных не удаётся, приложение таблиц пытается подключиться напрямую к этому файлу. Может быть указано в виде URI или системно‑специфической нотации пути к файлу. |
| [SourceType](../../aspose.cells.externalconnections/externalconnection/sourcetype/) { get; set; } | Получает или задаёт тип внешнего соединения DataSource. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid/) { get; set; } | Идентификатор для Single Sign On (SSO), используемый для аутентификации между промежуточным сервером spreadsheetML и внешним источником данных. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type/) { get; set; } | (**Устарело.**) Получает или задаёт тип внешнего соединения DataSource. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassExternalConnectionDemo
    {
        public static void Run()
        {
            string sourceDir = "Your Source Directory";

            Workbook workbook = new Workbook(sourceDir + "example.xlsx");
            ExternalConnectionCollection conns = workbook.DataConnections;
            foreach (ExternalConnection conn in conns)
            {
                if (conn is DBConnection dbConn)
                {
                    Console.WriteLine("Connection Info: " + dbConn.ConnectionInfo);
                    Console.WriteLine("Formula Definition: " + dbConn.PowerQueryFormula.FormulaDefinition);
                }
            }

            workbook = new Workbook(sourceDir + "example.xlsm");
            conns = workbook.DataConnections;
            foreach (ExternalConnection conn in conns)
            {
                if (conn is DBConnection dbConn)
                {
                    Console.WriteLine("Connection Info: " + dbConn.ConnectionInfo);
                    Console.WriteLine("Formula Definition: " + dbConn.PowerQueryFormula.FormulaDefinition);
                }
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


