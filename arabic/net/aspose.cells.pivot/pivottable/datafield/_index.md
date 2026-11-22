---
title: "PivotTable.DataField"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تحصل على كائن PivotField يمثل جميع حقول البيانات في جدول البيفوت. للقراءة فقط. يتم إنشاؤه فقط عندما يكون هناك حقلان بيانات أو أكثر في منطقة البيانات. بشكل افتراضي يكون في منطقة الصف. يمكنك سحبه إلى منطقة الصف/العمود باستخدام طريقة PivotTable.AddFieldToArea."
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/datafield/
---
## PivotTable.DataField property

يحصل على كائن [`PivotField`](../../pivotfield/) يمثل جميع حقول البيانات في جدول البيفوت. للقراءة فقط. يتم إنشاؤه فقط عندما يكون هناك حقلان بيانات أو أكثر في منطقة البيانات. بشكل افتراضي يكون في منطقة الصف. يمكنك سحبه إلى منطقة الصف/العمود باستخدام طريقة PivotTable.AddFieldToArea() .

```csharp
[Obsolete("Use PivotTable.ValuesField property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotField DataField { get; }
```

### ملاحظات

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotTable.ValuesField. ستُزال هذه الطريقة بعد 12 شهرًا منذ أكتوبر 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyDataFieldDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B4"].Value = 3000;

            // إنشاء جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // إضافة حقل الصف وحقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // الوصول وتعديل خصائص DataField
            // الموضع للقراءة فقط، لذا سنظهر خصائص أخرى
            pivotTable.DataField.DisplayName = "Total Sales";
            pivotTable.DataField.NumberFormat = "#,##0";
            
            // احفظ المصنف
            workbook.Save("PivotTableDataFieldDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


