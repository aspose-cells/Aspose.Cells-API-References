---
title: "CellsColor.ColorIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CellsColor. تحصل وتضبط فهرس اللون في لوحة الألوان. ينطبق فقط على اللون المفهرس"
type: docs
url: /ar/net/aspose.cells/cellscolor/colorindex/
---
## CellsColor.ColorIndex property

يحصل على فهرس اللون في لوحة الألوان ويضبطه. ينطبق فقط على اللون المفهرس.

```csharp
public int ColorIndex { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;

    public class CellsColorPropertyColorIndexDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحديد نطاق سنطبق عليه حدًا ملونًا
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:D4");

            // إنشاء مثال CellsColor
            CellsColor cellsColor = workbook.CreateCellsColor();

            // تعيين ColorIndex (فهرس اللوحة) – على سبيل المثال، 5
            cellsColor.ColorIndex = 5;

            // تطبيق CellsColor كلون الحد الداخلي للنطاق
            range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical,
                                   CellBorderType.Thin,
                                   cellsColor);

            // قراءة وعرض قيمة ColorIndex الحالية
            Console.WriteLine("Current ColorIndex value: " + cellsColor.ColorIndex);

            // احفظ المصنف لتصوّر النتيجة
            try
            {
                workbook.Save("ColorIndexDemo.xlsx");
                Console.WriteLine("Workbook saved as ColorIndexDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


