---
title: "ShapeTextAlignment.IsLockedText"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeTextAlignment özelliği. Çalışma sayfası korunduğunda şeklin kilitli olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing.texts/shapetextalignment/islockedtext/
---
## ShapeTextAlignment.IsLockedText property

Çalışma sayfası korunduğunda şeklin kilitli olup olmadığını gösterir.

```csharp
public bool IsLockedText { get; set; }
```

### Açıklamalar

Yalnızca çalışma sayfası korunduğunda çalışır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyIsLockedTextDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            Shape textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);
            textBox.Text = "Sample Text";

            // Metin hizalama özelliklerine erişin
            Aspose.Cells.Drawing.Texts.ShapeTextAlignment textAlignment = textBox.TextBody.TextAlignment;

            // IsLockedText özelliğini ayarlayın ve gösterin
            textAlignment.IsLockedText = true;
            Console.WriteLine("Text locked status: " + textAlignment.IsLockedText);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


