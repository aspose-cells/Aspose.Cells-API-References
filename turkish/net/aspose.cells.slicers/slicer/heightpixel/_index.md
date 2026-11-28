---
title: "Slicer.HeightPixel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Slicer özelliği. Belirtilen dilimleyicinin yüksekliğini piksel cinsinden alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.slicers/slicer/heightpixel/
---
## Slicer.HeightPixel property

Belirtilen dilimleyicinin yüksekliğini piksel cinsinden alır veya ayarlar.

```csharp
[Obsolete("Use Shape.Height property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int HeightPixel { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Shape.Height özelliğini kullanın. Bu özellik Mayıs 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

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

### Ayrıca Bakınız

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


