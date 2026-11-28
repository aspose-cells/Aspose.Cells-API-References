---
title: "ActiveXControl.IMEMode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ActiveXControl özelliği. Kontrol odaklandığında Giriş Yöntemi Düzenleyicisinin varsayılan çalışma zaman modunu alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/activexcontrol/imemode/
---
## ActiveXControl.IMEMode property

Kontrol odaklandığında Giriş Yöntemi Düzenleyicisinin varsayılan çalışma zaman modu alır ve ayarlar.

```csharp
public InputMethodEditorMode IMEMode { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlPropertyIMEModeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Uygun koordinatlarla bir ToggleButton ActiveX kontrolü ekle
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ToggleButton, 
                1, 1,  // Upper-left row/column
                1, 1,  // Upper-left row/column offsets
                100, 50);  // Width and height
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // IMEMode dahil olmak üzere özellikleri ayarla
            toggleButton.Caption = "ToggleButton1";
            toggleButton.PicturePosition = ControlPicturePositionType.AboveCenter;
            toggleButton.SpecialEffect = ControlSpecialEffectType.Sunken;
            toggleButton.IMEMode = InputMethodEditorMode.NoControl;

            // IMEMode özelliğini doğrula ve çıktısını al
            Console.WriteLine("ToggleButton IMEMode: " + toggleButton.IMEMode);

            // Çalışma kitabını kaydedin
            workbook.Save("ActiveXControlIMEModeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [InputMethodEditorMode](../../inputmethodeditormode/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


