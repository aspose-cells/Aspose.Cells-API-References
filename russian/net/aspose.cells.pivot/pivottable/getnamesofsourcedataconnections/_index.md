---
title: "PivotTable.GetNamesOfSourceDataConnections"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод PivotTable. Получает имена внешних соединений исходных данных"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/getnamesofsourcedataconnections/
---
## PivotTable.GetNamesOfSourceDataConnections method

Получает имена внешних соединений источников данных.

```csharp
public string[] GetNamesOfSourceDataConnections()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodGetNamesOfSourceDataConnectionsDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            sheet.Cells["A1"].Value = "Product";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["A2"].Value = "A";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["A3"].Value = "B";
            sheet.Cells["B3"].Value = 200;
            
            // Создать сводную таблицу и получить ссылку
            int pivotIndex = sheet.PivotTables.Add("PivotTable", "A1:B3", "C1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            // Получить соединения исходных данных
            string[] connections = pivotTable.GetNamesOfSourceDataConnections();
            
            // Вывести информацию о подключении
            Console.WriteLine("Pivot Table Source Data Connections:");
            foreach (string connection in connections)
            {
                Console.WriteLine(connection);
            }
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


