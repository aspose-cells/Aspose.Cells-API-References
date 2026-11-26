---
title: "Перечисление ConnectionDataSourceType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ExternalConnections.ConnectionDataSourceType. Указывает тип внешнего источника базы данных"
type: docs
url: /ru/net/aspose.cells.externalconnections/connectiondatasourcetype/
---
## ConnectionDataSourceType enumeration

Указывает тип внешнего источника базы данных

```csharp
public enum ConnectionDataSourceType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| ODBCBasedSource | `1` | Источник на основе ODBC |
| DAOBasedSource | `2` | Источник на основе DAO |
| FileBasedDataBaseSource | `3` | Источник базы данных на основе файлов |
| WebQuery | `4` | Веб‑запрос |
| OLEDBBasedSource | `5` | Источник на основе OLE DB |
| TextBasedSource | `6` | Источник на основе текста |
| ADORecordSet | `7` | Набор записей ADO |
| DSP | `8` | DSP |
| OLEDBDataModel | `100` | Источник данных OLE DB, созданный моделью данных электронной таблицы. |
| DataFeedDataModel | `101` | Источник данных потока данных, созданный моделью данных электронной таблицы. |
| WorksheetDataModel | `102` | Источник данных листа, созданный моделью данных электронной таблицы. |
| Table | `102` | Источник данных листа, созданный моделью данных электронной таблицы. |
| TextDataModel | `103` | Текстовый источник данных, созданный моделью данных электронной таблицы. |
| Unknown | `255` | Текстовый источник данных, созданный моделью данных электронной таблицы. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassConnectionDataSourceTypeDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные в лист
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Item1");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Item2");
            sheet.Cells["B3"].PutValue(2000);

            // Создать сводную таблицу, используя данные листа
            var pivotTable = sheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            
            // Получить соединение и продемонстрировать ConnectionDataSourceType
            var conn = sheet.PivotTables[0].GetSourceDataConnections()[0];
            Console.WriteLine("Connection Name: " + conn.Name);
            Console.WriteLine("Class Type: " + conn.ClassType);
            Console.WriteLine("Source Type: " + conn.SourceType);
            Console.WriteLine("Command: " + conn.Command);
            
            // Сохраните книгу
            workbook.Save("ExternalConnectionDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


