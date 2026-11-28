---
title: "TextBoxActiveXControl.BorderStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextBoxActiveXControl özelliği. Kontrol tarafından kullanılan kenarlık tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/borderstyle/
---
## TextBoxActiveXControl.BorderStyle property

Kontrol tarafından kullanılan kenarlık tipini alır ve ayarlar.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir ActiveX TextBox kontrolü ekle
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 1, 100, 100, 0);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // BorderStyle özelliğini ayarlayın
            textBox.BorderStyle = ControlBorderType.Single;

            // Çalışma kitabını kaydedin
            workbook.Save("TextBoxActiveXControlBorderStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ControlBorderType](../../controlbordertype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


