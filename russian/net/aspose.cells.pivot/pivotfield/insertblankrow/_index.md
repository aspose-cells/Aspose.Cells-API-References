---
title: "PivotField.InsertBlankRow"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Указывает, следует ли вставлять пустую строку после каждого элемента. Только для полей строк"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/insertblankrow/
---
## PivotField.InsertBlankRow property

Указывает, следует ли вставлять пустую строку после каждого элемента. Только для полей строк.

```csharp
public bool InsertBlankRow { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyInsertBlankRowDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["B1"].Value = "Quantity";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["B2"].Value = 10;
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["B3"].Value = 15;
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B4"].Value = 20;
            sheet.Cells["A5"].Value = "Apple";
            sheet.Cells["B5"].Value = 5;
            sheet.Cells["A6"].Value = "Orange";
            sheet.Cells["B6"].Value = 8;
            
            // Создать сводную таблицу
            int index = sheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Добавить поле строки и поле данных
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Установить свойство InsertBlankRow
            PivotField rowField = pivotTable.RowFields[0];
            rowField.InsertBlankRow = true;
            
            // Обновить и вычислить сводную таблицу
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Сохраните книгу
            workbook.Save("PivotFieldInsertBlankRowDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


