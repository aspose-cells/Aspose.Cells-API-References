---
title: "Slicer.NumberOfColumns"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Slicer. Возвращает или задаёт количество столбцов в срезе. Значение по умолчанию — 1"
type: docs
url: /ru/net/aspose.cells.slicers/slicer/numberofcolumns/
---
## Slicer.NumberOfColumns property

Возвращает или задает количество столбцов в slicer. Значение по умолчанию — 1.

```csharp
public int NumberOfColumns { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyNumberOfColumnsDemo
    {
        public static void Run()
        {
            // Создать книгу с образцовыми данными
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Создать примерные данные для сводной таблицы
            cells["A1"].Value = "Category";
            cells["B1"].Value = "Product";
            cells["A2"].Value = "Fruits";
            cells["B2"].Value = "Apple";
            cells["A3"].Value = "Fruits";
            cells["B3"].Value = "Banana";
            cells["A4"].Value = "Vegetables";
            cells["B4"].Value = "Carrot";

            // Создать сводную таблицу — сохранить индекс, затем получить объект PivotTable
            int pivotIndex = sheet.PivotTables.Add("D1", "A1:B4", "PivotTable");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Product");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Добавить срез, подключённый к сводной таблице
            int slicerIndex = sheet.Slicers.Add(pivotTable, "Category", "Slicer1");
            Slicer slicer = sheet.Slicers[slicerIndex];

            // Настроить свойства среза
            slicer.Caption = "Product Categories";
            slicer.TopPixel = 50;
            slicer.LeftPixel = 50;
            slicer.HeightPixel = 150;
            slicer.WidthPixel = 200;

            // Продемонстрировать свойство NumberOfColumns
            slicer.NumberOfColumns = 2;

            // Сохраните книгу
            workbook.Save("SlicerDemo.xlsx");
        }
    }
}
```

### См. также

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


