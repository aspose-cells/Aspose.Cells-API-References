---
title: "PivotTableCalculateOption.RefreshData"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTableCalculateOption. Указывает, следует ли обновлять источник данных сводной таблицы"
type: docs
url: /ru/net/aspose.cells.pivot/pivottablecalculateoption/refreshdata/
---
## PivotTableCalculateOption.RefreshData property

Указывает, обновляется ли источник данных сводной таблицы.

```csharp
public bool RefreshData { get; set; }
```

### Примечания

Если значение истинно, обновите кэш сводных данных из источника, затем вычислите все сводные таблицы на основе того же кэша.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionPropertyRefreshDataDemo
    {
        public static void Run()
        {
            // Создать книгу из исходного файла Excel
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Настройте примерные данные для сводной таблицы
            var cells = sheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Sales");
            cells["A2"].PutValue("A");
            cells["B2"].PutValue(100);
            cells["A3"].PutValue("B");
            cells["B3"].PutValue(200);
            cells["A4"].PutValue("C");
            cells["B4"].PutValue(300);

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Изменить исходные данные
            cells["B2"].PutValue(150); // Change value from 100 to 150

            // Вычислите сводную таблицу с опцией RefreshData
            PivotTableCalculateOption options = new PivotTableCalculateOption();
            options.RefreshData = true;
            pivotTable.CalculateData(options);

            // Выведите обновлённое значение сводной таблицы
            Console.WriteLine("Updated Pivot Table Value: " + cells["F5"].StringValue);
        }
    }
}
```

### См. также

* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


