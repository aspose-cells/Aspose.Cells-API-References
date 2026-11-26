---
title: "ExternalConnection.ClassType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Получает тип этого объекта ExternalConnection."
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/classtype/
---
## ExternalConnection.ClassType property

Получает тип этого объекта [`ExternalConnection`](../).

```csharp
public abstract ExternalConnectionClassType ClassType { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells[$"A{i}"].PutValue($"Product {i-1}");
                sheet.Cells[$"B{i}"].PutValue(i * 100);
            }

            // Создайте сводную таблицу с подключением к модели данных.
            int pivotIndex = sheet.PivotTables.Add("A1:B10", "C1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Получите внешнее соединение и продемонстрируйте свойство ClassType.
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            Console.WriteLine($"Connection ClassType: {conn.ClassType}");
            Console.WriteLine($"Expected ClassType: {ExternalConnectionClassType.DataModel}");

            // Сохраните книгу
            workbook.Save("ExternalConnectionClassTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


