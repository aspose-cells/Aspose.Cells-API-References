---
title: "Перечисление ExternalConnectionClassType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ExternalConnections.ExternalConnectionClassType. Представляет тип соединения"
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnectionclasstype/
---
## ExternalConnectionClassType enumeration

Представляет тип соединения

```csharp
public enum ExternalConnectionClassType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Database | `0` | ODBC или OLE DB |
| WebQuery | `1` | Веб‑запрос |
| TextBased | `2` | На основе текста |
| DataModel | `3` | Модель данных |
| Unkown | `4` |  |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ExternalConnectionsClassExternalConnectionClassTypeDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для соединения
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(i - 1);
                worksheet.Cells[$"B{i}"].PutValue($"Name_{i - 1}");
            }

            // Создать сводную таблицу с данными
            int pivotIndex = worksheet.PivotTables.Add("A1:B10", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Получить внешнее соединение и продемонстрировать свойства
            ExternalConnection conn = workbook.DataConnections[0];
            
            Console.WriteLine($"Connection Name: {conn.Name}");
            Console.WriteLine($"Class Type: {conn.ClassType}");
            Console.WriteLine($"Source Type: {conn.SourceType}");
            Console.WriteLine($"Command: {conn.Command}");
            Console.WriteLine($"Connection File: {conn.ConnectionFile ?? "null"}");
            Console.WriteLine($"Connection String: {conn.ConnectionString ?? "null"}");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


