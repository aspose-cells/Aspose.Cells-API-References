---
title: "Slicer.AlternativeText"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Slicer. Возвращает или задает описательную альтернативную текстовую строку объекта Slicer"
type: docs
url: /ru/net/aspose.cells.slicers/slicer/alternativetext/
---
## Slicer.AlternativeText property

Возвращает или задает описательную (альтернативную) текстовую строку объекта Slicer.

```csharp
[Obsolete("Use Shape.AlternativeText property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string AlternativeText { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте свойство [`AlternativeText`](../../../aspose.cells.drawing/shape/alternativetext/). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

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

### См. также

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


