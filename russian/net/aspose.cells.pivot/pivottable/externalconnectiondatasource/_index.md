---
title: "PivotTable.ExternalConnectionDataSource"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Получает внешний источник данных подключения"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/externalconnectiondatasource/
---
## PivotTable.ExternalConnectionDataSource property

Получает внешний источник данных подключения.

```csharp
[Obsolete("Use PivotTable.GetSourceDataConnections() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ExternalConnection ExternalConnectionDataSource { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Это свойство теперь устарело. Вместо него, пожалуйста, используйте метод PivotTable.GetSourceDataConnections(). Этот метод будет удалён через 12 месяцев, начиная с октября 2024 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyExternalConnectionDataSourceDemo
    {
        public static void Run()
        {
            // Создать книгу с внешним подключением данных
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Создать примерные данные
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B3"].PutValue(2000);

            // Добавьте сводную таблицу
            int index = sheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[index];

            // Получить внешнее подключение (только для чтения)
            ExternalConnection connection = pivot.ExternalConnectionDataSource;
            
            if (connection != null)
            {
                Console.WriteLine("Pivot table connection: " + connection.Name);
            }
            else
            {
                Console.WriteLine("No external connection found");
            }
        }
    }
}
```

### См. также

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


