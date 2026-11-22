---
title: "TextOptions.UnderlineColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextOptions. تحصل أو تعين لون الخط السفلي"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textoptions/underlinecolor/
---
## TextOptions.UnderlineColor property

الحصول أو تعيين لون الخط السفلي.

```csharp
public CellsColor UnderlineColor { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextOptionsPropertyUnderlineColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً يحتوي على نص لعرض خيارات النص
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 100);
            shape.Text = "Underline Color Demo";
            
            // احصل على TextOptions من الشكل
            TextOptions textOptions = shape.TextOptions;

            try
            {
                // اعرض قيمة UnderlineColor الحالية
                CellsColor currentColor = textOptions.UnderlineColor;
                Console.WriteLine($"Current UnderlineColor - Type: {currentColor.Type}, Color: {currentColor.Color}");

                // عيّن قيمة جديدة لـ UnderlineColor (نظرًا لأن الخاصية قابلة للقراءة والكتابة)
                CellsColor newColor = textOptions.UnderlineColor; // Use existing color object
                newColor.Color = System.Drawing.Color.Red;
                textOptions.UnderlineColor = newColor;

                // فعّل الخط السفلي لرؤية التأثير
                textOptions.Underline = FontUnderlineType.Single;

                // اعرض قيمة UnderlineColor الجديدة
                Console.WriteLine($"New UnderlineColor - Type: {textOptions.UnderlineColor.Type}, Color: {textOptions.UnderlineColor.Color}");

                // حفظ المصنف لرؤية التأثير
                workbook.Save("UnderlineColorDemo.xlsx");
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

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


