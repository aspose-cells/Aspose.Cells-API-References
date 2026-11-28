---
title: "ActiveXControlBase.LinkedCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ActiveXControlBase özelliği. Bağlı hücreyi alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/
---
## ActiveXControlBase.LinkedCell property

Bağlı hücreyi alır ve ayarlar.

```csharp
public string LinkedCell { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyLinkedCellDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı başlat
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına bir SpinButtonActiveXControl ekleyin
            Aspose.Cells.Drawing.Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton, 
                10, 10, 100, 30, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl spinButton = 
                (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;

            // SpinButton özelliklerini yapılandırın
            spinButton.Min = 0;
            spinButton.Max = 100;
            spinButton.Position = 50;
            spinButton.SmallChange = 1;

            // Kontrolü A1 hücresine bağlayın
            spinButton.LinkedCell = "A1";

            // A1 hücresinin değerini başlangıç konumuna eşit olacak şekilde ayarlayın
            workbook.Worksheets[0].Cells["A1"].PutValue(spinButton.Position);

            // Çalışma kitabını kaydedin
            workbook.Save("LinkedCellDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


