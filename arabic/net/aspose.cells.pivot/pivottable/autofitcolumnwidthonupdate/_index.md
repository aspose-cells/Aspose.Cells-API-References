---
title: "PivotTable.AutofitColumnWidthOnUpdate"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تشير إلى ما إذا كان سيتم ضبط عرض العمود تلقائيًا عند التحديث"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/autofitcolumnwidthonupdate/
---
## PivotTable.AutofitColumnWidthOnUpdate property

يشير إلى ما إذا كان يجب ضبط عرض العمود تلقائيًا عند التحديث

```csharp
public bool AutofitColumnWidthOnUpdate { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyAutofitColumnWidthOnUpdateDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("example.xlsx");
            
            // الوصول إلى ورقة العمل التي تحتوي على جدول البيفوت
            Worksheet worksheet = workbook.Worksheets["PIVOT"];
            
            // الوصول إلى PivotTable
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // تعطيل ضبط عرض العمود تلقائيًا عند التحديث
            pivotTable.AutofitColumnWidthOnUpdate = false;
            
            // تحديث جدول المحوري لتطبيق التغييرات
            worksheet.RefreshPivotTables();
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            Console.WriteLine("PivotTable AutofitColumnWidthOnUpdate property set successfully.");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


