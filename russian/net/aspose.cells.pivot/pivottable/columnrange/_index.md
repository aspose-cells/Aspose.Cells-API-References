---
title: "PivotTable.ColumnRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotTable. Возвращает объект CellArea, представляющий диапазон, содержащий область столбцов в отчете PivotTable. Только для чтения."
type: docs
url: /ru/net/aspose.cells.pivot/pivottable/columnrange/
---
## PivotTable.ColumnRange property

Возвращает объект CellArea, представляющий диапазон, содержащий область столбцов в отчете PivotTable. Только для чтения.

```csharp
public CellArea ColumnRange { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyColumnRangeDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Region";
            worksheet.Cells["C1"].Value = "Sales";
            
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = "North";
            worksheet.Cells["C2"].Value = 1000;
            
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = "South";
            worksheet.Cells["C3"].Value = 2000;
            
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = "East";
            worksheet.Cells["C4"].Value = 3000;
            
            // Создать сводную таблицу
            int index = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Добавить поля в сводную таблицу
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Обновить данные сводной таблицы
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Получить диапазон столбцов сводной таблицы
            CellArea columnRange = pivotTable.ColumnRange;
            Console.WriteLine("Pivot Table Column Range: " + columnRange);
            
            // Сохраните книгу
            workbook.Save("PivotTableColumnRangeDemo.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


