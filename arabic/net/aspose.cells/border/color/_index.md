---
title: "Border.Color"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Border. يحصل على أو يضبط لون الحد"
type: docs
url: /ar/net/aspose.cells/border/color/
---
## Border.Color property

يحصل أو يضبط لون الحد.

```csharp
public Color Color { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BorderPropertyColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى الخلية A1
            Cell cell = worksheet.Cells["A1"];
            
            // ضبط قيمة الخلية
            cell.PutValue("Border Color Demo");
            
            // احصل على نمط الخلية
            Style style = cell.GetStyle();
            
            // ضبط ألوان الحدود والأنماط
            style.Borders[BorderType.TopBorder].Color = Color.Red;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            
            style.Borders[BorderType.BottomBorder].Color = Color.Blue;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dotted;
            
            style.Borders[BorderType.LeftBorder].Color = Color.Green;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dashed;
            
            style.Borders[BorderType.RightBorder].Color = Color.FromArgb(255, 128, 0); // Orange
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            
            // تطبيق النمط على الخلية
            cell.SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("BorderColorDemo.xlsx");
            
            Console.WriteLine("Border color demo created successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


