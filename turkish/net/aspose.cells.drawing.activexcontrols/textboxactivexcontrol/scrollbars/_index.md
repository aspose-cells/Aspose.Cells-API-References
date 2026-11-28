---
title: "TextBoxActiveXControl.ScrollBars"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TextBoxActiveXControl özelliği. Kontrolün dikey kaydırma çubukları, yatay kaydırma çubukları, her ikisi ya da hiçbiri olup olmadığını belirtir"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/scrollbars/
---
## TextBoxActiveXControl.ScrollBars property

Denetimin dikey kaydırma çubukları, yatay kaydırma çubukları, her ikisi ya da hiçbiri olup olmadığını belirtir.

```csharp
public ControlScrollBarType ScrollBars { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyScrollBarsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Yeni bir şekil koleksiyonu oluştur ve ActiveX kontrolü ekle
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 1, 1, 200, 100);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;
            
            // ScrollBars özelliğini dikeye ayarla
            textBox.ScrollBars = ControlScrollBarType.BarsVertical;
            
            // Çalışma kitabını kaydedin
            workbook.Save("TextBoxScrollBarsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ControlScrollBarType](../../controlscrollbartype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


