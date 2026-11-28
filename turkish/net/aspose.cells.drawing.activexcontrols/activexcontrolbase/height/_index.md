---
title: "ActiveXControlBase.Height"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ActiveXControlBase özelliği. Kontrolün yüksekliğini puan biriminde alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/height/
---
## ActiveXControlBase.Height property

Kontrolün yüksekliğini nokta biriminde alır ve ayarlar.

```csharp
public virtual double Height { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyHeightDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı başlat
            Workbook workbook = new Workbook();

            // Bir RadioButton ActiveXControl ekle
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 0, 100, 50);
            RadioButtonActiveXControl activeXControl = (RadioButtonActiveXControl)shape.ActiveXControl;

            // Temel özellikleri ayarlayın
            activeXControl.Caption = "Height Demo";
            activeXControl.IsAutoSize = false; // Disable auto-size to demonstrate Height property

            // Height özelliğini göster
            Console.WriteLine("Original Height: " + activeXControl.Height);
            activeXControl.Height = 75;
            Console.WriteLine("Modified Height: " + activeXControl.Height);

            // Çalışma kitabını kaydedin
            workbook.Save("ActiveXControlHeightDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


