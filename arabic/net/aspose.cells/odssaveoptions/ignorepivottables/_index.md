---
title: "OdsSaveOptions.IgnorePivotTables"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OdsSaveOptions. تشير إلى ما إذا كان يتم حفظ الجداول المحورية"
type: docs
url: /ar/net/aspose.cells/odssaveoptions/ignorepivottables/
---
## OdsSaveOptions.IgnorePivotTables property

يشير إلى ما إذا كان يتم حفظ جداول المحور.

```csharp
public bool IgnorePivotTables { get; set; }
```

### ملاحظات

ميزة الجداول المحورية في OpenOffice لديها إعدادات أقل مقارنةً بـ Excel، لذا فإن نتائج الجداول المحورية تختلف كثيرًا. أحيانًا يكون من الأفضل تجاهل هذه الجداول المحورية عند حفظ ملف .ods

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class OdsSaveOptionsPropertyIgnorePivotTablesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(3000);

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = workbook.Worksheets[0].PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // إنشاء مثيل OdsSaveOptions
            OdsSaveOptions saveOptions = new OdsSaveOptions();

            // عرض قيمة IgnorePivotTables الحالية
            Console.WriteLine("Current IgnorePivotTables value: " + saveOptions.IgnorePivotTables);

            // ضبط لتجاهل الجداول المحورية عند الحفظ
            saveOptions.IgnorePivotTables = true;

            // حفظ مع تجاهل الجداول المحورية
            workbook.Save("IgnorePivotTablesDemo_Ignored.ods", saveOptions);

            // ضبط لتضمين الجداول المحورية عند الحفظ
            saveOptions.IgnorePivotTables = false;

            // حفظ مع تضمين الجداول المحورية
            workbook.Save("IgnorePivotTablesDemo_Included.ods", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


