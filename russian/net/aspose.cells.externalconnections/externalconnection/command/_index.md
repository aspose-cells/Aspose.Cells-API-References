---
title: "ExternalConnection.Command"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Строка, содержащая команду базы данных, которую необходимо передать API поставщика данных, который будет взаимодействовать с внешним источником для получения данных"
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/command/
---
## ExternalConnection.Command property

Строка, содержащая команду базы данных, передаваемую API поставщика данных, который будет взаимодействовать с внешним источником для получения данных

```csharp
public virtual string Command { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте лист и некоторые примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(150);
            
            // Создайте диапазон таблицы
            var range = worksheet.Cells.CreateRange("A1:B3");
            
            // Создайте сводную таблицу, используя диапазон в качестве источника
            int index = worksheet.PivotTables.Add("D1", "A1:B3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[index];
            
            // Получить внешние соединения
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // Отобразить свойство Command соединения
            if (connections.Length > 0)
            {
                Console.WriteLine("Connection Command: " + connections[0].Command);
            }
            
            // Сохраните книгу
            workbook.Save("ExternalConnectionCommandDemo.xlsx");
        }
    }
}
```

### См. также

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


