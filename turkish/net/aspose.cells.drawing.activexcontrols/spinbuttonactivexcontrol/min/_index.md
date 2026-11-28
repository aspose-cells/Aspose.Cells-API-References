---
title: "SpinButtonActiveXControl.Min"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SpinButtonActiveXControl özelliği. Kabul edilebilir minimum değeri alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min/
---
## SpinButtonActiveXControl.Min property

Minimum kabul edilebilir değeri alır ve ayarlar.

```csharp
public int Min { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyMinDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bir SpinButton ActiveX kontrolü ekle
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 1, 0, 1, 0, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl spinButton = 
                (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            
            // SpinButton'ın Min özelliğini ayarla
            spinButton.Min = 0;
            
            // İşlevselliği göstermek için diğer özellikleri ayarla
            spinButton.Max = 100;
            spinButton.Position = 50;
            
            // Çalışma kitabını kaydedin
            workbook.Save("SpinButtonMinDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


