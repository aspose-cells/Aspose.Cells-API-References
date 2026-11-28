---
title: "SpinButtonActiveXControl.Max"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SpinButtonActiveXControl özelliği. Kabul edilebilir maksimum değeri alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max/
---
## SpinButtonActiveXControl.Max property

Maksimum kabul edilebilir değeri alır ve ayarlar.

```csharp
public int Max { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyMaxDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bir SpinButton ActiveX kontrolü ekle
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 1, 1, 1, 100, 30);
            
            // ActiveX denetimini al ve Max özelliğini ayarla
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.Max = 100;
            
            // Çalışma kitabını kaydedin
            workbook.Save("SpinButtonMaxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


