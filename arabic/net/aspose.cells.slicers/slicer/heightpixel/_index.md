---
title: "Slicer.HeightPixel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Slicer. تُرجع أو تعين ارتفاع الـ Slicer المحدد بوحدات البكسل"
type: docs
url: /ar/net/aspose.cells.slicers/slicer/heightpixel/
---
## Slicer.HeightPixel property

تُرجع أو تعين ارتفاع الـ Slicer المحدد، بوحدات البكسل.

```csharp
[Obsolete("Use Shape.Height property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int HeightPixel { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية Shape.Height. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerPropertyHeightPixelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["A4"].Value = "C";

            int tableIndex = worksheet.ListObjects.Add("A1", "A4", true);
            ListObject table = worksheet.ListObjects[tableIndex];

            int slicerIndex = worksheet.Slicers.Add(table, 0, "D1");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            slicer.HeightPixel = 150;

            workbook.Save("SlicerHeightDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


