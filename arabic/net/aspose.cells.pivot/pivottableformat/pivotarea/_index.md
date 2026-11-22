---
title: "PivotTableFormat.PivotArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTableFormat. تحصل على منطقة المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivottableformat/pivotarea/
---
## PivotTableFormat.PivotArea property

يحصل على منطقة الجدول المحوري.

```csharp
public PivotArea PivotArea { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableFormatPropertyPivotAreaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);

            // إنشاء جدول محوري
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // إضافة حقول إلى مناطق pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // احصل على تنسيق المحور وقم بتكوين منطقة المحور الخاصة به
            int formatIndex = pivotTable.PivotFormats.Add();
            PivotTableFormat pivotFormat = pivotTable.PivotFormats[formatIndex];
            PivotArea pivotArea = pivotFormat.PivotArea;
            
            // تعيين خصائص منطقة المحور
            pivotArea.AxisType = PivotFieldType.Data;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;

            // إنشاء وتطبيق نمط على منطقة المحور
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            pivotFormat.SetStyle(style);

            // احفظ المصنف
            workbook.Save("PivotTableWithPivotArea.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotArea](../../pivotarea/)
* class [PivotTableFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


