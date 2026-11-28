---
title: "ComboBoxActiveXControl.HideSelection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ComboBoxActiveXControl özelliği. Kontrol odaklanmadığında seçili metnin vurgulanıp vurgulanmadığını gösterir."
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/hideselection/
---
## ComboBoxActiveXControl.HideSelection property

Kontrol odaklanmadığında seçili metnin vurgulanıp vurgulanmadığını gösterir.

```csharp
public bool HideSelection { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyHideSelectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tüm gerekli parametrelerle bir ComboBox ActiveX kontrolü ekle
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                10, 10, 150, 30, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Temel özellikleri yapılandırın
            comboBox.ListRows = 5;
            comboBox.Value = "Select an item";
            
            // Doğru özellik adını kullanarak örnek öğeler ekle
            comboBox.ListFillRange = "A1:A3"; // Alternative way to set items
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // HideSelection özelliğini göster
            comboBox.HideSelection = true; // Text won't show selection highlight when control loses focus

            // Çalışma kitabını kaydedin
            workbook.Save("ComboBoxHideSelectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


