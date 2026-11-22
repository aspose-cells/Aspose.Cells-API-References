---
title: "الفئة PivotTableFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Pivot.PivotTableFormat. تمثل التنسيق المحدد في جدول محوري"
type: docs
url: /ar/net/aspose.cells.pivot/pivottableformat/
---
## PivotTableFormat class

يمثل التنسيق المحدد في جدول محوري.

```csharp
public class PivotTableFormat
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [PivotArea](../../aspose.cells.pivot/pivottableformat/pivotarea/) { get; } | يحصل على منطقة الجدول المحوري. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetStyle](../../aspose.cells.pivot/pivottableformat/getstyle/)() | يحصل على النمط المنسق. |
| [SetStyle](../../aspose.cells.pivot/pivottableformat/setstyle/)(Style) | يضبط نمط منطقة الجدول المحوري. |

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotTableFormatDemo
    {
        public static void RunDemo()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);

            // إضافة جدول محوري
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // الوصول إلى PivotTableFormatCollection
            PivotTableFormatCollection pivotFormats = pivotTable.PivotFormats;

            // إضافة تنسيق جديد إلى المجموعة
            int formatIndex = pivotFormats.Add();
            PivotTableFormat pivotFormat = pivotFormats[formatIndex];

            // الوصول إلى PivotArea في التنسيق
            PivotArea pivotArea = pivotFormat.PivotArea;
            pivotArea.AxisType = PivotFieldType.Data;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;

            // إنشاء نمط جديد
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // تطبيق النمط على PivotTableFormat
            pivotFormat.SetStyle(style);

            // احفظ المصنف
            workbook.Save("PivotTableFormatDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


