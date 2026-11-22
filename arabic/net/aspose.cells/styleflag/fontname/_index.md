---
title: "StyleFlag.FontName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعداد اسم الخط"
type: docs
url: /ar/net/aspose.cells/styleflag/fontname/
---
## StyleFlag.FontName property

سيتم تطبيق إعداد اسم الخط.

```csharp
public bool FontName { get; set; }
```

### أمثلة

```csharp
using System;
using System.Data;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء بيانات نموذجية
            cells["A1"].PutValue("Product Name");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Laptop");
            cells["B2"].PutValue(999.99);
            cells["A3"].PutValue("Phone");
            cells["B3"].PutValue(699.99);

            // إنشاء أنماط بأسماء خطوط مختلفة
            Style headerStyle = workbook.CreateStyle();
            headerStyle.Font.Name = "Arial";
            headerStyle.Font.IsBold = true;
            headerStyle.Font.Size = 14;

            Style priceStyle = workbook.CreateStyle();
            priceStyle.Font.Name = "Courier New";
            priceStyle.Custom = "$#,##0.00";

            // تطبيق نمط الرأس باستخدام StyleFlag
            Aspose.Cells.Range headerRange = cells.CreateRange(0, 0, 1, 2);
            StyleFlag headerFlag = new StyleFlag();
            headerFlag.FontName = true;
            headerFlag.FontBold = true;
            headerFlag.FontSize = true;
            headerRange.ApplyStyle(headerStyle, headerFlag);

            // تطبيق نمط السعر باستخدام StyleFlag مع التركيز على FontName
            Aspose.Cells.Range priceRange = cells.CreateRange(1, 1, 2, 1);
            StyleFlag priceFlag = new StyleFlag();
            priceFlag.FontName = true;
            priceFlag.NumberFormat = true;
            priceRange.ApplyStyle(priceStyle, priceFlag);

            // ضبط الأعمدة تلقائيًا لتحسين الرؤية
            worksheet.AutoFitColumns();

            // احفظ المصنف
            workbook.Save("FontNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


