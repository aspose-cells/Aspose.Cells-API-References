---
title: "PivotTable.PreserveFormatting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تُشير إلى ما إذا كان تنسيق الخلايا PivotTableFormat يُحفظ عندما يتم تحديث أو إعادة حساب PivotTable"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/preserveformatting/
---
## PivotTable.PreserveFormatting property

تشير إلى ما إذا كان تنسيق الخلايا ([`PivotTableFormat`](../../pivottableformat/)) يُحفظ عندما يتم تحديث أو إعادة حساب PivotTable.

```csharp
[Obsolete("Use PivotTable.PreserveCellFormattingOnUpdate property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool PreserveFormatting { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotTable.PreserveCellFormattingOnUpdate. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ يوليو 2026. تُعرب Aspose عن أسفها لأي إزعاج قد تكون قد تعرضت له.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPreserveFormattingDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("source.xlsx");
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى أول جدول محوري
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // تمكين حفظ التنسيق أثناء التحديث
            pivotTable.PreserveFormatting = true;
            
            // تطبيق بعض التنسيق على منطقة بيانات جدول المحور
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 10;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            // تنسيق منطقة بيانات جدول المحور
            pivotTable.FormatAll(style);
            
            // تحديث وحساب بيانات جدول البيفوت
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


