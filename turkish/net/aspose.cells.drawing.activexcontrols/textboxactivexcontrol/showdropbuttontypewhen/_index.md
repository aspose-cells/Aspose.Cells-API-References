---
title: "TextBoxActiveXControl.ShowDropButtonTypeWhen"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextBoxActiveXControl özelliği. Açılır düğmede gösterilen sembolü belirtir"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/showdropbuttontypewhen/
---
## TextBoxActiveXControl.ShowDropButtonTypeWhen property

Açılır düğmede görüntülenen sembolü belirtir

```csharp
public ShowDropButtonType ShowDropButtonTypeWhen { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyShowDropButtonTypeWhenDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir ActiveX TextBox kontrolü ekle
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.TextBox, 
                1, 1, 1, 1, 100, 50);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // ShowDropButtonTypeWhen özelliğini ayarla
            textBox.ShowDropButtonTypeWhen = ShowDropButtonType.Focus;

            // Çalışma kitabını kaydedin
            workbook.Save("TextBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ShowDropButtonType](../../showdropbuttontype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


