---
title: "PivotField.ShowAllItems"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Указывает, следует ли отображать все элементы в представлении сводной таблицы, даже если они не содержат сводных данных. Значение по умолчанию — false."
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/showallitems/
---
## PivotField.ShowAllItems property

Указывает, следует ли отображать все элементы в представлении PivotTable, даже если они не содержат сводных данных. Значение по умолчанию — false.

```csharp
public bool ShowAllItems { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowAllItemsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Пример данных для сводной таблицы
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Product");
            sheet.Cells["C1"].PutValue("Sales");
            
            sheet.Cells["A2"].PutValue("Electronics");
            sheet.Cells["B2"].PutValue("Laptop");
            sheet.Cells["C2"].PutValue(1200);
            
            sheet.Cells["A3"].PutValue("Electronics");
            sheet.Cells["B3"].PutValue("Phone");
            sheet.Cells["C3"].PutValue(800);
            
            sheet.Cells["A4"].PutValue("Furniture");
            sheet.Cells["B4"].PutValue("Chair");
            sheet.Cells["C4"].PutValue(150);

            // Добавьте сводную таблицу
            int index = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Установить свойство ShowAllItems для поля строки
            PivotField rowField = pivotTable.RowFields[0];
            rowField.ShowAllItems = true;

            // Вычислите данные и сохраните
            pivotTable.CalculateData();
            workbook.Save("PivotFieldShowAllItemsDemo.xlsx");
        }
    }
}
```

### См. также

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


