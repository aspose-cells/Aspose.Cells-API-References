---
title: "ComboBoxActiveXControl.BorderOleColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ComboBoxActiveXControl özelliği. Arka planın ole rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/borderolecolor/
---
## ComboBoxActiveXControl.BorderOleColor property

Arka planın ole rengini alır ve ayarlar.

```csharp
public int BorderOleColor { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyBorderOleColorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasını al
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir ComboBox ActiveX denetimi ekle
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                1, 1, 100, 20, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Temel özellikleri yapılandırın
            comboBox.BorderStyle = Aspose.Cells.Drawing.ActiveXControls.ControlBorderType.Single;
            
            // BorderOleColor özelliğini göster
            comboBox.BorderOleColor = ColorTranslator.ToOle(Color.Red); // Set border color to red
            
            // Bazı örnek metin ayarla
            comboBox.Value = "Border Color Demo";

            // Çalışma kitabını kaydedin
            workbook.Save("ComboBoxBorderColorDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


