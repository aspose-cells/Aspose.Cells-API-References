---
title: "TextBoxOptions.AllowTextToOverflow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextBoxOptions özelliği. Metnin şekli aşmasına izin verilip verilmeyeceği"
type: docs
url: /tr/net/aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/
---
## TextBoxOptions.AllowTextToOverflow property

Metnin şekli taşmasına izin verilip verilmeyeceği.

```csharp
public bool AllowTextToOverflow { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxOptionsPropertyAllowTextToOverflowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir metin kutusu ekle
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 50);

            // Aşabilir metni ayarla
            textBox.Text = "This is a long text that might overflow the text box boundaries if AllowTextToOverflow is false";

            // Metin aşımını etkinleştir
            textBox.TextBoxOptions.AllowTextToOverflow = true;

            // Çalışma kitabını kaydedin
            workbook.Save("TextBoxAllowTextToOverflowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TextBoxOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


