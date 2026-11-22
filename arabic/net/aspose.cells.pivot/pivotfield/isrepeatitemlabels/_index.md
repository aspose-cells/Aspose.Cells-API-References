---
title: "PivotField.IsRepeatItemLabels"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. تشير إلى ما إذا كان يجب تكرار تسميات الحقل في منطقة الصف أو العمود. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/isrepeatitemlabels/
---
## PivotField.IsRepeatItemLabels property

يحدد ما إذا كان يجب تكرار تسميات الحقل في منطقة الصف أو العمود. القيمة الافتراضية هي false.

```csharp
public bool IsRepeatItemLabels { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsRepeatItemLabelsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("example.xlsx");

            // الوصول إلى ورقة العمل التي تحتوي على جدول البيفوت
            Worksheet worksheet = workbook.Worksheets["Actual"];

            // الوصول إلى PivotTable
            PivotTable pivotTable = worksheet.PivotTables[0];

            // تمكين تكرار تسميات العناصر لحقل الصف الأول
            pivotTable.RowFields[0].IsRepeatItemLabels = true;

            // تمكين تكرار تسميات العناصر لحقل العمود الأول
            pivotTable.ColumnFields[0].IsRepeatItemLabels = true;

            // احفظ المصنف المعدل
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


