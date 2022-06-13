---
title: QueryTable
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет информацию QueryTable.
type: docs
weight: 4930
url: /ru/net/aspose.cells/querytable/
---
## QueryTable class

Представляет информацию QueryTable.

```csharp
public class QueryTable
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [AdjustColumnWidth](../../aspose.cells/querytable/adjustcolumnwidth) { get; set; } | Возвращает или задает AdjustColumnWidth объекта. |
| [ConnectionId](../../aspose.cells/querytable/connectionid) { get; } | Получает идентификатор соединения таблицы запросов. |
| [ExternalConnection](../../aspose.cells/querytable/externalconnection) { get; } | Получает связанное внешнее соединение. |
| [Name](../../aspose.cells/querytable/name) { get; } | Получает имя таблицы запросов. |
| [PreserveFormatting](../../aspose.cells/querytable/preserveformatting) { get; set; } | Возвращает или задает PreserveFormatting объекта. |
| [ResultRange](../../aspose.cells/querytable/resultrange) { get; } | Получает диапазон результата. |

### Примеры

```csharp

[C#]

  //Создание экземпляра рабочей книги object
Workbook workbook = new Workbook();

//Получение ссылки на первый worksheet
Worksheet worksheet = workbook.Worksheets[0];
  //Получение первой таблицы запросов в worksheet
QueryTable qt = worksheet.QueryTables[0];
  //Получение отображаемого адреса таблицы запросов.
string address = qt.ResultRange.Address;

[VB.NET]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()

'Obtaining the reference of the first worksheet
Dim worksheet As Worksheet = workbook.Worksheets(0)
'Getting the first query table in the worksheet
QueryTable qt = worksheet.QueryTables[0];
'Getting display address of the query table.
string address = qt.ResultRange.Address;
```

### Смотрите также

* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->