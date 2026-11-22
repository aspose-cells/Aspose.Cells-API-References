---
title: "PivotOptions.DropZoneCategories"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotOptions. تحدد ما إذا كان التحكم لكل حقل PivotTable على محور صف PivotTable في PivotTable المصدر يظهر على المخطط عندما تكون الخاصية dropZonesVisible مضبوطة على true"
type: docs
url: /ar/net/aspose.cells.charts/pivotoptions/dropzonecategories/
---
## PivotOptions.DropZoneCategories property

يحدد ما إذا كان عنصر التحكم لكل حقل PivotTable على محور الصفوف في PivotTable المصدر يظهر على المخطط عندما تكون الخاصية dropZonesVisible مُعينة إلى true.

```csharp
public bool DropZoneCategories { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneCategoriesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف ورقة عمل وبعض البيانات النموذجية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            
            // إضافة مخطط يستخدم بيانات pivot
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // الوصول إلى خيارات pivot من المخطط
            PivotOptions options = chart.PivotOptions;
            
            // عرض خاصية DropZoneCategories
            options.DropZoneCategories = true;
            Console.WriteLine("DropZoneCategories enabled: " + options.DropZoneCategories);
            
            // احفظ المصنف
            workbook.Save("PivotOptionsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


