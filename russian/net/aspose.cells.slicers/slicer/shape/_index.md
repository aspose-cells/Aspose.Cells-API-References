---
title: "Slicer.Shape"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Slicer. Возвращает объект Shape, связанный с указанным срезом. Только для чтения"
type: docs
url: /ru/net/aspose.cells.slicers/slicer/shape/
---
## Slicer.Shape property

Возвращает объект Shape, связанный с указанным слайсером. Только для чтения.

```csharp
public SlicerShape Shape { get; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Slicers;
    using Aspose.Cells.Pivot;
    using System;

    public class SlicerPropertyShapeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для сводной таблицы
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 300;

            // Создайте сводную таблицу
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Добавить слайсер
            int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "FruitSlicer");
            Slicer slicer = worksheet.Slicers[slicerIndex];

            try
            {
                // Получить доступ к свойству Shape (только для чтения)
                var slicerShape = slicer.Shape;

                // Отобразить информацию о объекте Shape
                Console.WriteLine("Slicer Shape Type: " + slicerShape.GetType().Name);
                Console.WriteLine("Slicer Shape Name: " + slicerShape.Name);
                Console.WriteLine("Slicer Shape Width: " + slicerShape.Width);
                Console.WriteLine("Slicer Shape Height: " + slicerShape.Height);

                // Сохраните книгу
                workbook.Save("SlicerShapeDemo.xlsx");
                Console.WriteLine("Slicer Shape has been demonstrated and saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [SlicerShape](../../../aspose.cells.drawing/slicershape/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


