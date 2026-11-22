---
title: "StyleFlag.TopBorder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعدادات الحد العلوي"
type: docs
url: /ar/net/aspose.cells/styleflag/topborder/
---
## StyleFlag.TopBorder property

سيتم تطبيق إعدادات الحد العلوي.

```csharp
public bool TopBorder { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyTopBorderDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء نمط بإعدادات الحد العلوي
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].Color = Color.Red;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Dashed;

            // إنشاء علم نمط وتمكين تعديل الحد العلوي
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.TopBorder = true;

            // تطبيق النمط على الخلية A1 مع تمكين علم الحد العلوي فقط
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Text");
            cell.SetStyle(style, styleFlag);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


