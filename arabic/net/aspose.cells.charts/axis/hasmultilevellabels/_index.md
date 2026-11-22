---
title: "Axis.HasMultiLevelLabels"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية المحور. تشير إلى ما إذا كان يجب عرض التسميات كمستوى متعدد"
type: docs
url: /ar/net/aspose.cells.charts/axis/hasmultilevellabels/
---
## Axis.HasMultiLevelLabels property

يشير إلى ما إذا كان يجب عرض التسميات كمستويات متعددة.

```csharp
public bool HasMultiLevelLabels { get; set; }
```

### ملاحظات

صالح فقط لمحور الفئة.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyHasMultiLevelLabelsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة مع فئات متعددة المستويات
            worksheet.Cells["A1"].PutValue("Main Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Sub Category");
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue("Carrot");
            worksheet.Cells["C1"].PutValue("Value");
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(8);
            
            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط بما في ذلك الفئات متعددة المستويات
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "A1:B3";
            
            // التحقق من خاصية HasMultiLevelLabels وعرضها
            Console.WriteLine("HasMultiLevelLabels: " + chart.CategoryAxis.HasMultiLevelLabels);
            
            // احفظ المصنف
            workbook.Save("AxisPropertyHasMultiLevelLabelsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


