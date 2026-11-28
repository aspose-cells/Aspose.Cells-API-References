---
title: "ToggleButtonActiveXControl.Picture"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ToggleButtonActiveXControl özelliği. Resmin verisini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/picture/
---
## ToggleButtonActiveXControl.Picture property

Resmin verilerini alır ve ayarlar.

```csharp
public byte[] Picture { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir ToggleButton ActiveX kontrolü ekleyin ve onun ActiveXControl özelliğini alın
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ToggleButton, 1, 1, 100, 30, 100, 30);
            var toggleButton = (Aspose.Cells.Drawing.ActiveXControls.ToggleButtonActiveXControl)shape.ActiveXControl;

            // Toggle düğmesi için resmi ayarla
            byte[] data = File.ReadAllBytes("image.png");
            toggleButton.Picture = data;

            // Çalışma kitabını kaydedin
            workbook.Save("ToggleButtonWithPicture.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


