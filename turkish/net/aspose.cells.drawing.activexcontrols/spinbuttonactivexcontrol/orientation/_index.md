---
title: "SpinButtonActiveXControl.Orientation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SpinButtonActiveXControl özelliği. SpinButton veya ScrollBar'ın dikey mi yoksa yatay mı yönlendirildiğini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/orientation/
---
## SpinButtonActiveXControl.Orientation property

SpinButton veya ScrollBar'ın dikey mi yoksa yatay mı yönlendirildiğini alır ve ayarlar.

```csharp
public ControlScrollOrientation Orientation { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyOrientationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir SpinButton ActiveX kontrolü ekleyin
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 100, 50, 100, 50);
            SpinButtonActiveXControl spinButton = (SpinButtonActiveXControl)shape.ActiveXControl;

            // Yönlendirmeyi kontrol et ve değiştir
            if (spinButton.Orientation == ControlScrollOrientation.Auto)
            {
                spinButton.Orientation = ControlScrollOrientation.Horizontal;
            }

            // Çalışma kitabını kaydedin
            workbook.Save("SpinButtonOrientationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ControlScrollOrientation](../../controlscrollorientation/)
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


