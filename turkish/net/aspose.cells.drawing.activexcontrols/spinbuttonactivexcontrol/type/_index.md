---
title: "SpinButtonActiveXControl.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SpinButtonActiveXControl özelliği. ActiveX denetiminin tipini alır"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/type/
---
## SpinButtonActiveXControl.Type property

ActiveX denetiminin türünü alır.

```csharp
public override ControlType Type { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir SpinButton ActiveX denetimi ekle (parametreler: left, top, width, height)
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 100, 30, 100, 30);
            SpinButtonActiveXControl spinButton = (SpinButtonActiveXControl)shape.ActiveXControl;
            
            // Denetim tipini Type özelliği kullanarak kontrol et
            if (spinButton.Type == ControlType.SpinButton)
            {
                // SpinButton'a özgü bazı özellikleri ayarla
                spinButton.Min = 0;
                spinButton.Max = 100;
                spinButton.Position = 50;
                spinButton.SmallChange = 1;
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("SpinButtonActiveXControlDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ControlType](../../controltype/)
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


