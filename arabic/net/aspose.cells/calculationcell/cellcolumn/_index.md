---
title: "CalculationCell.CellColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationCell. تحصل على فهرس العمود للخلية"
type: docs
url: /ar/net/aspose.cells/calculationcell/cellcolumn/
---
## CalculationCell.CellColumn property

يحصل على فهرس العمود للخلية.

```csharp
public int CellColumn { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationCellPropertyCellColumnDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أدخل بعض البيانات وصيغة بسيطة
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // احصل على مثال CalculationCell عبر الانعكاس (منشئه غير عام)
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell), 
                    nonPublic: true);

                // قراءة وعرض قيمة خاصية CellColumn
                Console.WriteLine("CellColumn value: " + calcCell.CellColumn);

                // عرض إضافي للخصائص ذات الصلة (اختياري)
                Console.WriteLine("CellRow value: " + calcCell.CellRow);
                Console.WriteLine("Workbook is null: " + (calcCell.Workbook == null));
                Console.WriteLine("Worksheet is null: " + (calcCell.Worksheet == null));

                // احفظ المصنف (سيحتوي الملف على البيانات التي أضفناها)
                workbook.Save("CellColumnDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


