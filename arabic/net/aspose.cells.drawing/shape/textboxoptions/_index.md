---
title: "Shape.TextBoxOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل على معلومات النص داخل الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/shape/textboxoptions/
---
## Shape.TextBoxOptions property

يحصل على معلومات النص في الشكل

```csharp
public TextBoxOptions TextBoxOptions { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;

    public class ShapePropertyTextBoxOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مربع نص
            int textBoxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textBox = worksheet.TextBoxes[textBoxIndex];
            textBox.Text = "This is a sample text box to demonstrate TextBoxOptions properties.";

            // اعرض خصائص TextBoxOptions الحالية
            TextBoxOptions textBoxOptions = textBox.TextBoxOptions;
            Console.WriteLine("Current TextBoxOptions:");
            Console.WriteLine("Vertical Alignment: " + textBoxOptions.ShapeTextVerticalAlignment);
            Console.WriteLine("Resize To Fit Text: " + textBoxOptions.ResizeToFitText);
            Console.WriteLine("Text Direction: " + textBoxOptions.ShapeTextDirection);
            Console.WriteLine("Left Margin: " + textBoxOptions.LeftMarginPt + " pt");
            Console.WriteLine("Right Margin: " + textBoxOptions.RightMarginPt + " pt");

            // عدّل خصائص TextBoxOptions
            textBoxOptions.ShapeTextVerticalAlignment = ShapeTextVerticalAlignmentType.Middle;
            textBoxOptions.ResizeToFitText = true;
            textBoxOptions.ShapeTextDirection = TextVerticalType.Vertical;
            textBoxOptions.LeftMarginPt = 10;
            textBoxOptions.RightMarginPt = 10;
            textBoxOptions.TopMarginPt = 5;
            textBoxOptions.BottomMarginPt = 5;

            // احفظ المصنف
            workbook.Save("TextBoxOptionsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextBoxOptions](../../../aspose.cells.drawing.texts/textboxoptions/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


