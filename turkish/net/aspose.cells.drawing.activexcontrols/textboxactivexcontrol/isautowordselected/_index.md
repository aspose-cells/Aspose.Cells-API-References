---
title: "TextBoxActiveXControl.IsAutoWordSelected"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextBoxActiveXControl özelliği. Seçimi genişletmek için kullanılan temel birimi belirtir. True, temel birimin tek bir karakter olduğunu belirtir. false, temel birimin bütün bir kelime olduğunu belirtir"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isautowordselected/
---
## TextBoxActiveXControl.IsAutoWordSelected property

Bir seçimi genişletmek için kullanılan temel birimi belirtir. True, temel birimin tek bir karakter olduğunu belirtir. false, temel birimin tam bir kelime olduğunu belirtir.

```csharp
public virtual bool IsAutoWordSelected { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyIsAutoWordSelectedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape textBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 0, 0, 1, 1, 200, 30);
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)textBoxShape.ActiveXControl;

            Console.WriteLine("Initial IsAutoWordSelected: " + textBoxControl.IsAutoWordSelected);

            if (!textBoxControl.IsAutoWordSelected)
            {
                textBoxControl.IsAutoWordSelected = true;
            }

            Console.WriteLine("Final IsAutoWordSelected: " + textBoxControl.IsAutoWordSelected);
        }
    }
}
```

### Ayrıca Bakınız

* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


