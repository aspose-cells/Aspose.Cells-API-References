---
title: "PivotTable.ShowValuesRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Указывает, отображается ли строка значений"
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/showvaluesrow/
---
## PivotTable.ShowValuesRow property

Указывает, показывать ли строку значений.

```csharp
public bool ShowValuesRow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowValuesRowDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Настройте сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit as row
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Quantity as data
            
            // Продемонстрировать свойство ShowValuesRow
            Console.WriteLine("Initial ShowValuesRow: " + pivotTable.ShowValuesRow);
            pivotTable.ShowValuesRow = true;
            Console.WriteLine("After setting to true: " + pivotTable.ShowValuesRow);
            
            // Сохраните книгу
            workbook.Save("PivotTableShowValuesRowDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


