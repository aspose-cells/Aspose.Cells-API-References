---
title: "Format3D.HasTopBevelData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Format3D method. تشير إلى ما إذا كان الشكل يحتوي على بيانات الحافة العلوية"
type: docs
url: /ar/net/aspose.cells.drawing/format3d/hastopbeveldata/
---
## Format3D.HasTopBevelData method

يشير إلى ما إذا كان الشكل يحتوي على بيانات الحافة العلوية.

```csharp
public bool HasTopBevelData()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class Format3DMethodHasTopBevelDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // إنشاء مخطط ثلاثي الأبعاد
            int chartIndex = sheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // احصل على تنسيق 3D
            Format3D format3D = chart.NSeries[0].ShapeProperties.Format3D;

            // تعيين الحافة العلوية
            format3D.TopBevel.Type = BevelPresetType.Circle;
            format3D.TopBevel.Width = 6;
            format3D.TopBevel.Height = 6;

            // تحقق وعرض بيانات الحافة
            if (format3D.HasTopBevelData())
            {
                Console.WriteLine("Top Bevel Type: " + format3D.TopBevel.Type);
                Console.WriteLine("Top Bevel Width: " + format3D.TopBevel.Width);
                Console.WriteLine("Top Bevel Height: " + format3D.TopBevel.Height);
            }

            workbook.Save("Format3DTopBevelDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


