---
title: "Slicer.AlternativeText"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Slicer. تُرجع أو تُعيّن سلسلة النص البديل الوصفي لكائن Slicer"
type: docs
url: /ar/net/aspose.cells.slicers/slicer/alternativetext/
---
## Slicer.AlternativeText property

تُرجع أو تُعيّن سلسلة النص الوصفي (البديل) لكائن Slicer.

```csharp
[Obsolete("Use Shape.AlternativeText property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string AlternativeText { get; set; }
```

### ملاحظات

ملاحظة: هذه العضو الآن مهجور. بدلاً من ذلك، يرجى استخدام خاصية [`AlternativeText`](../../../aspose.cells.drawing/shape/alternativetext/). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Slicers;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class SlicerPropertyAlternativeTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            
            ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1:A3", "", true)];
            table.DisplayName = "Table1";

            int slicerIndex = worksheet.Slicers.Add(table, 0, "C1");
            Slicer slicer = worksheet.Slicers[slicerIndex];
            slicer.AlternativeText = "AlternativeText test";

            workbook.Save("SlicerAlternativeTextDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


