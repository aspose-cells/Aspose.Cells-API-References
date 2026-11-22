---
title: "StyleFlag.BottomBorder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعدادات الحدود السفلية"
type: docs
url: /ar/net/aspose.cells/styleflag/bottomborder/
---
## StyleFlag.BottomBorder property

سيتم تطبيق إعدادات الحد السفلي.

```csharp
public bool BottomBorder { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyBottomBorderDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء نمط بإعدادات الحدود السفلية
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.BottomBorder].Color = Color.Red;

            // إنشاء علم النمط وتمكين تعديل الحد السفلي
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.BottomBorder = true;

            // تطبيق النمط مع العلم على الخلية A1
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Cell with bottom border");
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


