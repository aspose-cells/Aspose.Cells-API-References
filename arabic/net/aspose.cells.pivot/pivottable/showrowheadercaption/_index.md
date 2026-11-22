---
title: "PivotTable.ShowRowHeaderCaption"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تشير إلى ما إذا كان عنوان رأس الصف يُظهر في تقرير PivotTable. تشير إلى ما إذا كان يتم عرض عناوين الحقول وقوائم الفلاتر المنسدلة"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/showrowheadercaption/
---
## PivotTable.ShowRowHeaderCaption property

تشير إلى ما إذا كان عنوان رأس الصف يُظهر في تقرير PivotTable. تشير إلى ما إذا كان يتم عرض عناوين الحقول وقوائم الفلاتر المنسدلة

```csharp
[Obsolete("Use PivotTable.ShowHeaders property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ShowRowHeaderCaption { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotTable.ShowHeaders. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ أبريل 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowRowHeaderCaptionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل وتعبئتها ببيانات عينة
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // إضافة بيانات عينة لجدول محوري
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // تكوين جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // عرض خاصية ShowRowHeaderCaption
            pivotTable.ShowRowHeaderCaption = true;
            Console.WriteLine("Row Header Caption Visible: " + pivotTable.ShowRowHeaderCaption);
            
            // احفظ المصنف
            workbook.Save("PivotTableShowRowHeaderCaptionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


