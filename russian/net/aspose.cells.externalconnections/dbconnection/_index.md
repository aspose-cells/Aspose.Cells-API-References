---
title: DBConnection
second_title: Справочник по Aspose.Cells для .NET API
description: Задает все свойства связанные с подключением к внешним данным ODBC или OLE DB.
type: docs
weight: 3280
url: /ru/net/aspose.cells.externalconnections/dbconnection/
---
## DBConnection class

Задает все свойства, связанные с подключением к внешним данным ODBC или OLE DB.

```csharp
public class DBConnection : ExternalConnection
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [BackgroundRefresh](../../aspose.cells.externalconnections/externalconnection/backgroundrefresh) { get; set; } | Указывает, может ли соединение обновляться в фоновом режиме (асинхронно). true, если предпочтительным использованием соединения является асинхронное обновление в фоновом режиме; false, если предпочтительным использованием соединения является синхронное обновление на переднем плане. |
| [Command](../../aspose.cells.externalconnections/dbconnection/command) { get; set; } | Строка, содержащая команду базы данных для передачи API-интерфейсу поставщика данных, который будет взаимодействовать с внешним источником для извлечения data |
| [CommandType](../../aspose.cells.externalconnections/dbconnection/commandtype) { get; set; } | Указывает тип команды OLE DB. 1. Запрос указывает имя куба 2. Запрос задает оператор SQL 3. Запрос задает имя таблицы 4. Запрос указывает, что была предоставлена информация по умолчанию, а интерпретация зависит от поставщика. 5. Запрос против веб-поставщик данных списка. |
| [ConnectionDescription](../../aspose.cells.externalconnections/externalconnection/connectiondescription) { get; set; } | Указывает описание пользователя для этого подключения |
| [ConnectionId](../../aspose.cells.externalconnections/externalconnection/connectionid) { get; } | Указывает уникальный идентификатор этого соединения. |
| [ConnectionInfo](../../aspose.cells.externalconnections/dbconnection/connectioninfo) { get; set; } | Строка информации о подключении используется для связи с источником данных OLE DB или ODBC. |
| [CredentialsMethodType](../../aspose.cells.externalconnections/externalconnection/credentialsmethodtype) { get; set; } | Указывает метод проверки подлинности, который будет использоваться при установлении (или повторном установлении) соединения. |
| [Id](../../aspose.cells.externalconnections/externalconnection/id) { get; } | Получает идентификатор соединения. |
| [IsDeleted](../../aspose.cells.externalconnections/externalconnection/isdeleted) { get; set; } | Указывает, было ли удалено связанное подключение к книге. true, если соединение было удалено; в противном случае false. |
| [IsNew](../../aspose.cells.externalconnections/externalconnection/isnew) { get; set; } | Истинно, если соединение не обновлялось в первый раз; в противном случае ложно. Это состояние может произойти, когда пользователь сохраняет файл до завершения запроса. |
| [KeepAlive](../../aspose.cells.externalconnections/externalconnection/keepalive) { get; set; } | Истинно, когда приложение для работы с электронными таблицами должно прилагать усилия для поддержания соединения открытым. При значении false приложение должно закрыть соединение после получения информации . |
| [Name](../../aspose.cells.externalconnections/externalconnection/name) { get; set; } | Указывает имя соединения. Каждое соединение должно иметь уникальное имя. |
| [OdcFile](../../aspose.cells.externalconnections/externalconnection/odcfile) { get; set; } | Указывает полный путь к файлу внешнего подключения, из которого это подключение было создано. Если во время попытки обновления данных происходит сбой подключения, а reconnectionMethod=1, , приложение для работы с электронными таблицами попытается повторить попытку, используя информацию из внешнего файла подключения вместо объекта подключения, встроенного в книгу. |
| [OnlyUseConnectionFile](../../aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile) { get; set; } | Указывает, должно ли приложение электронных таблиц всегда и только использовать информацию о соединении во внешнем файле соединения, указанном атрибутом odcFile , при обновлении соединения. Если false, то приложение электронной таблицы должно следовать процедуре, указанной атрибутом reconnectionMethod . |
| [Parameters](../../aspose.cells.externalconnections/externalconnection/parameters) { get; } | получает[`ConnectionParameterCollection`](../connectionparametercollection) для ODBC или веб-запроса. |
| override [PowerQueryFormula](../../aspose.cells.externalconnections/dbconnection/powerqueryformula) { get; } | Получает определение формулы мощного запроса. |
| [ReconnectionMethodType](../../aspose.cells.externalconnections/externalconnection/reconnectionmethodtype) { get; set; } | Указывает, что должно делать приложение для работы с электронными таблицами при сбое подключения. Значение по умолчанию — ReConnectionMethodType.Required. |
| [RefreshInternal](../../aspose.cells.externalconnections/externalconnection/refreshinternal) { get; set; } | Указывает количество минут между автоматическими обновлениями соединения. |
| [RefreshOnLoad](../../aspose.cells.externalconnections/externalconnection/refreshonload) { get; set; } | Истинно, если это соединение должно обновляться при открытии файла; в противном случае false. |
| [SaveData](../../aspose.cells.externalconnections/externalconnection/savedata) { get; set; } | Истинно, если внешние данные, полученные через соединение для заполнения таблицы, должны быть сохранены вместе с рабочей книгой; в противном случае ложно. |
| [SavePassword](../../aspose.cells.externalconnections/externalconnection/savepassword) { get; set; } | Истинно, если пароль должен быть сохранен как часть строки подключения; в противном случае False. |
| [SeverCommand](../../aspose.cells.externalconnections/dbconnection/severcommand) { get; set; } | Указывает вторую текстовую строку команды, которая сохраняется, когда используются поля страницы на основе сервера сводной таблицы. Для подключений ODBC serverCommand обычно является более широким запросом, чем команда (в первом нет предложения WHERE). На основе этих двух команд (Command и ServerCommand) можно заполнить пользовательский интерфейс параметров и построить параметризованные запросы |
| [SourceFile](../../aspose.cells.externalconnections/externalconnection/sourcefile) { get; set; } | Используется, когда внешний источник данных основан на файлах. При сбое подключения к такому источнику данных приложение для работы с электронными таблицами пытается напрямую подключиться к этому файлу. Может быть , выраженным в URI или системной нотации пути к файлу. |
| [SSOId](../../aspose.cells.externalconnections/externalconnection/ssoid) { get; set; } | Идентификатор для единого входа (SSO), используемый для аутентификации между промежуточным сервером электронной таблицыML и внешним источником данных. |
| [Type](../../aspose.cells.externalconnections/externalconnection/type) { get; set; } | Получает или задает тип источника данных внешнего подключения. |

### Смотрите также

* class [ExternalConnection](../externalconnection)
* пространство имен [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
