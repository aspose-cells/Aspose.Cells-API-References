---
title: "PivotField.NonAutoSortDefault"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. تشير إلى ما إذا كانت عملية الفرز التي سيتم تطبيقها على هذا الحقل المحوري هي عملية فرز تلقائي أم فرز بيانات بسيط"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/nonautosortdefault/
---
## PivotField.NonAutoSortDefault property

تشير إلى ما إذا كانت عملية الفرز التي سيتم تطبيقها على هذا الحقل المحوري هي عملية فرز تلقائي أم فرز بيانات بسيط.

```csharp
[Obsolete("Use !PivotField.SortSetting.IsSimpleSort property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool NonAutoSortDefault { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام الخاصية !PivotField.SortSetting.IsSimpleSort. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyNonAutoSortDefaultDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("example.xlsx");
            
            // الوصول إلى ورقة العمل الأولى وجدول المحور
            Worksheet worksheet = workbook.Worksheets[0];
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // الوصول إلى حقل الصف الأول في جدول المحور
            PivotField pivotField = pivotTable.RowFields[0];
            
            // تعيين خاصية NonAutoSortDefault إلى true
            pivotField.NonAutoSortDefault = true;
            
            // إخراج قيمة الخاصية
            Console.WriteLine("NonAutoSortDefault property value: " + pivotField.NonAutoSortDefault);
            
            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


