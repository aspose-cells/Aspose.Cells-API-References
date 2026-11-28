---
title: "TextBoxOptions.WrapTextInShape"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextBoxOptions özelliği. Bir şekil içinde metin kaydırmayı belirtir. False  Metin gövdesinde kaydırma olmaz. True  Metin gövdesinde kaydırma olur."
type: docs
url: /tr/net/aspose.cells.drawing.texts/textboxoptions/wraptextinshape/
---
## TextBoxOptions.WrapTextInShape property

Şekil içinde metin kaydırmayı belirtir. False - Metin gövdesinde kaydırma olmaz. True - Metin gövdesinde kaydırma olur.

```csharp
public bool WrapTextInShape { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyWrapTextInShapeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir metin kutusu şekli ekleyin
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);

            // Şekil içinde kaydırılacak metni ayarla
            textBox.Text = "This is a long text that should wrap within the text box shape boundaries when WrapTextInShape is enabled.";

            // Şekil içinde metin kaydırmayı etkinleştir
            textBox.TextBoxOptions.WrapTextInShape = true;

            // Çalışma kitabını kaydedin
            workbook.Save("TextBoxWrapTextDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


