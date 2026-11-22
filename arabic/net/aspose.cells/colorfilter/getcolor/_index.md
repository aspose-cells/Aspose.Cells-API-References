---
title: "ColorFilter.GetColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ColorFilter. يحصل على لون هذا الفلتر"
type: docs
url: /ar/net/aspose.cells/colorfilter/getcolor/
---
## ColorFilter.GetColor method

يحصل على لون هذا الفلتر.

```csharp
public Color GetColor(WorksheetCollection sheets)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الأوراق | WorksheetCollection |  |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColorFilterMethodGetColorWithWorksheetCollectionDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["A4"].PutValue("Item 3");
            
            // إنشاء مرشح تلقائي
            worksheet.AutoFilter.Range = "A1:A4";
            
            // إنشاء تصفية لون
            CellsColor color = workbook.CreateCellsColor();
            color.Color = Color.Red;
            worksheet.AutoFilter.AddFillColorFilter(0, BackgroundType.Solid, color, color);
            worksheet.AutoFilter.Refresh();
            
            // احصل على مرشح اللون وتحقق من لونه
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            ColorFilter colorFilter = filterColumn.Filter as ColorFilter;
            
            if (colorFilter != null)
            {
                Color retrievedColor = colorFilter.GetColor(workbook.Worksheets);
                Console.WriteLine("Filter color: " + retrievedColor.ToString());
            }
        }
    }
}
```

### انظر أيضًا

* class [WorksheetCollection](../../worksheetcollection/)
* class [ColorFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


