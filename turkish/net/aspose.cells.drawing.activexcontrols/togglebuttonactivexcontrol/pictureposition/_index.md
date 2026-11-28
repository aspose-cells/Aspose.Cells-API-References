---
title: "ToggleButtonActiveXControl.PicturePosition"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ToggleButtonActiveXControl özelliği. Kontrolün resminin konumunu başlığına göre alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/pictureposition/
---
## ToggleButtonActiveXControl.PicturePosition property

Kontrolün resminin konumunu başlığına göre alır ve ayarlar.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyPicturePositionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tüm gerekli parametrelerle bir ToggleButton ActiveX kontrolü ekleyin
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 100, 30, 0);
            var control = shape.ActiveXControl;

            if (control is ToggleButtonActiveXControl toggleButton)
            {
                // PicturePosition özelliğini ayarla
                toggleButton.PicturePosition = ControlPicturePositionType.AboveLeft;

                // İşlevselliği göstermek için diğer özellikleri ayarla
                toggleButton.Caption = "Toggle Button";
                toggleButton.Picture = new byte[0]; // Empty picture for demo
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ToggleButtonActiveXControlDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


