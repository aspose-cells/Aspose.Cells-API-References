---
title: "StyleFlag.RightBorder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعدادات الحد الأيمن"
type: docs
url: /ar/net/aspose.cells/styleflag/rightborder/
---
## StyleFlag.RightBorder property

سيتم تطبيق إعدادات الحد الأيمن.

```csharp
public bool RightBorder { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyRightBorderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نمط مع حدود
            Style borderStyle = workbook.CreateStyle();
            borderStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            borderStyle.Borders[BorderType.RightBorder].Color = System.Drawing.Color.Red;

            // إنشاء علم نمط وتمكين الحد الأيمن
            StyleFlag borderFlag = new StyleFlag();
            borderFlag.RightBorder = true;

            // تطبيق النمط على خلية
            Cell cell = worksheet.Cells["B2"];
            cell.SetStyle(borderStyle, borderFlag);

            // احفظ المصنف
            workbook.Save("RightBorderDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


