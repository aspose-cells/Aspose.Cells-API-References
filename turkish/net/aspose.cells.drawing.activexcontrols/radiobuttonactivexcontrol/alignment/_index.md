---
title: "RadioButtonActiveXControl.Alignment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RadioButtonActiveXControl özelliği. Başlığın kontrolle ilişkili konumunu alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/alignment/
---
## RadioButtonActiveXControl.Alignment property

Altyazının denetime göre konumunu alır ve ayarlar.

```csharp
public ControlCaptionAlignmentType Alignment { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyAlignmentDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Yeni bir şekil koleksiyonu oluştur ve ActiveX kontrolü ekle
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddActiveXControl(ControlType.RadioButton, 1, 1, 100, 30, 0, 0);
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape.ActiveXControl;
            
            // Alignment özelliğini ayarla
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            
            // Çalışma kitabını kaydedin
            workbook.Save("RadioButtonAlignmentDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ControlCaptionAlignmentType](../../controlcaptionalignmenttype/)
* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


