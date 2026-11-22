---
title: "PivotField.IsAscendShow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. تشير إلى ما إذا كان حقل PivotTable المحدد يُظهر تلقائيًا بترتيب تصاعدي"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/isascendshow/
---
## PivotField.IsAscendShow property

يشير إلى ما إذا كان حقل PivotTable المحدد يُعرض تلقائيًا بترتيب تصاعدي.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.IsTop property or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAscendShow { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن قديمة. بدلاً من ذلك، يرجى استخدام الخاصية PivotField.Top10AutoShowSettings.IsTop أو طريقة PivotField.Top10AutoShow() بدلاً من ذلك. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAscendShowDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;

            // إضافة جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];
            
            // تعيين خاصية IsAscendShow
            rowField.IsAscendShow = true;
            Console.WriteLine("IsAscendShow (Row Field): " + rowField.IsAscendShow);
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[0];
            
            // تعيين خاصية IsAscendShow
            dataField.IsAscendShow = false;
            Console.WriteLine("IsAscendShow (Data Field): " + dataField.IsAscendShow);
            
            // تحديث جدول المحور
            pivotTable.RefreshData();
            pivotTable.CalculateData();
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


