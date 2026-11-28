---
title: "SpinButtonActiveXControl.Position"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SpinButtonActiveXControl özelliği. Değeri alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/position/
---
## SpinButtonActiveXControl.Position property

Değeri alır ve ayarlar.

```csharp
public int Position { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyPositionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir SpinButton ActiveX kontrolü ekleyin
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton,
                1, 0, 1, 0, 100, 30);

            // ActiveX kontrolünü al ve Position özelliğini ayarla
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.Position = 30;

            // Çalışma kitabını kaydedin
            workbook.Save("SpinButtonPositionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


