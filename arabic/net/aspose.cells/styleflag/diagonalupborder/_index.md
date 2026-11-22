---
title: "StyleFlag.DiagonalUpBorder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعدادات الحد القطري الصاعد"
type: docs
url: /ar/net/aspose.cells/styleflag/diagonalupborder/
---
## StyleFlag.DiagonalUpBorder property

سيتم تطبيق إعدادات الحدود القطرية العلوية.

```csharp
public bool DiagonalUpBorder { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleFlagPropertyDiagonalUpBorderDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية A1 وتعيين بعض النص
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // إنشاء كائن نمط وتعيين الحد القطري الصاعد
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.DiagonalUp].Color = Color.FromArgb(255, 0, 0, 255);

            // إنشاء علم نمط وتمكين علم الحد القطري الصاعد
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.DiagonalUpBorder = true;

            // تطبيق النمط مع العلم على الخلية
            cell.SetStyle(style, styleFlag);

            // إنشاء خلية أخرى لتوضيح التأثير
            Cell cell2 = worksheet.Cells["B2"];
            cell2.PutValue("Diagonal Up Border Demo");

            // إنشاء نمط مختلف للمقارنة
            Style style2 = workbook.CreateStyle();
            style.Borders[BorderType.DiagonalUp].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.DiagonalUp].Color = Color.FromArgb(255, 0, 255, 0);

            // تطبيق النمط الثاني باستخدام العلم نفسه
            cell2.SetStyle(style2, styleFlag);

            // احفظ المصنف
            workbook.Save("StyleFlagPropertyDiagonalUpBorderDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


