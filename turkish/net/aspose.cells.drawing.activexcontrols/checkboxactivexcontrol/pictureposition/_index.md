---
title: "CheckBoxActiveXControl.PicturePosition"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CheckBoxActiveXControl özelliği. Kontrolün resminin konumunu başlığına göre alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/pictureposition/
---
## CheckBoxActiveXControl.PicturePosition property

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
    public class CheckBoxActiveXControlPropertyPicturePositionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tüm gerekli parametrelerle bir CheckBox ActiveX kontrolü ekleyin
            var shape = worksheet.Shapes.AddActiveXControl(
                ControlType.CheckBox, 
                10,  // left
                10,  // top
                150, // width
                30,  // height
                0,   // leftOffset
                0    // topOffset
            );
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // CheckBox özelliklerini yapılandırın
            checkBox.Caption = "Sample CheckBox";
            checkBox.PicturePosition = ControlPicturePositionType.Center;
            checkBox.IsAutoSize = true;

            // Çalışma kitabını kaydedin
            workbook.Save("CheckBoxPicturePositionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


