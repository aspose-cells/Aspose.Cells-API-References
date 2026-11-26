---
title: "Перечисление OLEDBCommandType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.ExternalConnections.OLEDBCommandType enum. Указывает тип команды OLE DB"
type: docs
url: /ru/net/aspose.cells.externalconnections/oledbcommandtype/
---
## OLEDBCommandType enumeration

Указывает тип команды OLE DB.

```csharp
public enum OLEDBCommandType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Тип команды не указан. |
| CubeName | `1` | Указывает имя куба |
| SqlStatement | `2` | Указывает оператор SQL |
| TableName | `3` | Указывает имя таблицы |
| DefaultInformation | `4` | Указывает, что предоставлена информация по умолчанию, и как её интерпретировать, зависит от провайдера. |
| WebBasedList | `5` | Указывает запрос, который направлен к веб‑основному поставщику данных списка. |
| TableCollection | `6` | Указывает список таблиц. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassOLEDBCommandTypeDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Получить внешнее соединение
            ExternalConnectionCollection connections = workbook.DataConnections;
            ExternalConnection conn = connections[0];
            
            // Продемонстрировать использование OLEDBCommandType
            Console.WriteLine("Connection Name: " + conn.Name);
            Console.WriteLine("Source Type: " + conn.SourceType);
            Console.WriteLine("Command Type: " + conn.CommandType);
            Console.WriteLine("Command: " + conn.Command);
            
            // Изменить тип команды и продемонстрировать
            conn.CommandType = OLEDBCommandType.TableName;
            Console.WriteLine("\nAfter changing CommandType:");
            Console.WriteLine("Command Type: " + conn.CommandType);
            
            // Сохраните книгу
            workbook.Save("OLEDBCommandTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


