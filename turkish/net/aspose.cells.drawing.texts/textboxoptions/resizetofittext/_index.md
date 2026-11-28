---
title: "TextBoxOptions.ResizeToFitText"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextBoxOptions özelliği. Şekli metne sığacak şekilde yeniden boyutlandırıp boyutlandırmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textboxoptions/resizetofittext/
---
## TextBoxOptions.ResizeToFitText property

Şekli metne sığdırmak için yeniden boyutlandırıp boyutlandırmayacağını gösterir

```csharp
public bool ResizeToFitText { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyResizeToFitTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir metin kutusu oluştur
            Aspose.Cells.Drawing.TextBox textBox = worksheet.Shapes.AddTextBox(1, 1, 100, 100, 200, 50);
            textBox.Text = "This is a sample text that will make the text box resize to fit";

            // TextBoxOptions'ı doğru şekilde eriş
            textBox.TextBoxOptions.ResizeToFitText = true;

            // Çalışma kitabını kaydedin
            workbook.Save("TextBoxResizeToFitTextDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


