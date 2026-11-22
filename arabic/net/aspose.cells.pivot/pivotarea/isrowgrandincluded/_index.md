---
title: "PivotArea.IsRowGrandIncluded"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotArea. تشير إلى ما إذا كان إجمالي الصف شاملًا"
type: docs
url: /ar/net/aspose.cells.pivot/pivotarea/isrowgrandincluded/
---
## PivotArea.IsRowGrandIncluded property

يشير إلى ما إذا كان إجمالي الصف الإجمالي مشمولًا.

```csharp
public bool IsRowGrandIncluded { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyIsRowGrandIncludedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // بيانات عينة
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);

            // إنشاء جدول محوري
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // إضافة حقول
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // إنشاء تنسيق محوري
            int formatIndex = pivotTable.PivotFormats.Add();
            PivotTableFormat pivotFormat = pivotTable.PivotFormats[formatIndex];
            PivotArea pivotArea = pivotFormat.PivotArea;
            
            // عرض مثال على خاصية IsRowGrandIncluded
            pivotArea.AxisType = PivotFieldType.Data;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = false;

            // تطبيق نمط لتسليط الضوء على الصف الإجمالي
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGreen;
            style.Pattern = BackgroundType.Solid;
            pivotFormat.SetStyle(style);

            workbook.Save("PivotAreaIsRowGrandIncludedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


