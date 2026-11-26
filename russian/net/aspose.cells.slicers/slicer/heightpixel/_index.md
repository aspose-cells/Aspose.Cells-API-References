---
title: "Slicer.HeightPixel"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Slicer property. Возвращает или задает высоту указанного среза в пикселях"
type: docs
url: /ru/net/aspose.cells.slicers/slicer/heightpixel/
---
## Slicer.HeightPixel property

Возвращает или задает высоту указанного среза в пикселях.

```csharp
[Obsolete("Use Shape.Height property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int HeightPixel { get; set; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте свойство Shape.Height. Это свойство будет удалено через 12 месяцев, начиная с мая 2025 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

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

### См. также

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


