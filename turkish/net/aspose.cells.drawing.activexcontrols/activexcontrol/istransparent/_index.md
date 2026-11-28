---
title: "ActiveXControl.IsTransparent"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ActiveXControl özelliği. Kontrolün şeffaf olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/
---
## ActiveXControl.IsTransparent property

Kontrolün şeffaf olup olmadığını belirtir.

```csharp
public bool IsTransparent { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIsTransparentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle ActiveX kontrolünü barındıracak bir şekil oluştur
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Label, 
                1, 1, 200, 50, 
                0, 0); // Adding missing parameters for upperLeftRow, upperLeftColumn, height, width, left, top

            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            // Kontrol özelliklerini ayarla
            label.Caption = "Sample Label";
            label.IsTransparent = false; // Demonstrating IsTransparent property

            // IsTransparent özelliğini doğrula ve çıktısını al
            Console.WriteLine("Label IsTransparent property: " + label.IsTransparent);

            // Şeffaflığı değiştir ve tekrar doğrula
            label.IsTransparent = true;
            Console.WriteLine("Label IsTransparent property after change: " + label.IsTransparent);

            // Çalışma kitabını kaydedin
            workbook.Save("ActiveXControlIsTransparentDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


