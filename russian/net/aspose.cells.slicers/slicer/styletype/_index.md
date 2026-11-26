---
title: "Slicer.StyleType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Slicer. Укажите тип встроенного стиля среза. Тип по умолчанию — SlicerStyleLight1"
type: docs
url: /ru/net/aspose.cells.slicers/slicer/styletype/
---
## Slicer.StyleType property

Укажите тип встроенного стиля слайсера. Тип по умолчанию — SlicerStyleLight1.

```csharp
public SlicerStyleType StyleType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerPropertyStyleTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(20);

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Добавить поле строки
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);

            // Добавить срез
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "A1", "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            // Установить свойства среза, включая StyleType
            slicer.StyleType = SlicerStyleType.SlicerStyleDark2;
            slicer.Caption = "Fruit Selection";
            slicer.NumberOfColumns = 2;
            slicer.Width = 200;
            slicer.Height = 100;

            // Сохраните книгу
            workbook.Save("SlicerStyleTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [SlicerStyleType](../../slicerstyletype/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


