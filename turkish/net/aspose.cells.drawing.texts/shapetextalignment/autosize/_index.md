---
title: "ShapeTextAlignment.AutoSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeTextAlignment özelliği. Şeklin boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing.texts/shapetextalignment/autosize/
---
## ShapeTextAlignment.AutoSize property

Şeklin boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir.

```csharp
public bool AutoSize { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyAutoSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir metin kutusu şekli ekle
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 100, 200);
            textBox.Text = "This is a sample text that will demonstrate AutoSize property functionality";

            // Metin hizalamasını alın
            ShapeTextAlignment shapeTextAlignment = textBox.TextBody.TextAlignment;

            // AutoSize = false (varsayılan) gösterin
            shapeTextAlignment.AutoSize = false;
            Console.WriteLine("AutoSize false - Fixed size: " + textBox.Width + "x" + textBox.Height);

            // AutoSize = true gösterin
            shapeTextAlignment.AutoSize = true;
            Console.WriteLine("AutoSize true - Auto sized: " + textBox.Width + "x" + textBox.Height);

            // Çalışma kitabını kaydedin
            workbook.Save("ShapeTextAlignmentAutoSizeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


