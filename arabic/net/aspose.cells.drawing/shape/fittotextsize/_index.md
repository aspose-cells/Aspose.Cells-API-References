---
title: "Shape.FitToTextSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Shape. إعادة حساب مساحة النص المناسبة لعرض جميع محتوى النص"
type: docs
url: /ar/net/aspose.cells.drawing/shape/fittotextsize/
---
## Shape.FitToTextSize method

إعادة حساب منطقة نص مناسبة لعرض جميع محتويات النص.

```csharp
public void FitToTextSize()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeMethodFitToTextSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مربع نص
            Shape textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 100);
            textBox.Text = "This is a sample text that will demonstrate the FitToTextSize method functionality.";

            try
            {
                // عرض الأبعاد الأصلية
                Console.WriteLine($"Original Width: {textBox.Width}, Height: {textBox.Height}");

                // استدعاء طريقة FitToTextSize
                textBox.FitToTextSize();

                // عرض الأبعاد المعدلة
                Console.WriteLine($"Adjusted Width: {textBox.Width}, Height: {textBox.Height}");
                Console.WriteLine("FitToTextSize method executed successfully");

                // إضافة المزيد من النص لإظهار التأثير
                textBox.Text += " Adding more text to show how the shape adjusts to fit the content.";
                textBox.FitToTextSize();
                Console.WriteLine($"Final Width: {textBox.Width}, Height: {textBox.Height}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FitToTextSize method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("ShapeMethodFitToTextSizeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


