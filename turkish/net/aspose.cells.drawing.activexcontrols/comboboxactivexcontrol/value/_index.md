---
title: "ComboBoxActiveXControl.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ComboBoxActiveXControl özelliği. Kontrolün değerini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/value/
---
## ComboBoxActiveXControl.Value property

Denetimin değerini alır ve ayarlar.

```csharp
public string Value { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir ComboBox ActiveX denetimi ekle
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 1, 1, 0, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // ComboBox için özellikleri ayarla
            comboBox.Value = "Initial Value";
            comboBox.ListFillRange = "A1:A3";
            
            // Liste aralığına bazı örnek veriler ekle
            worksheet.Cells["A1"].PutValue("Option 1");
            worksheet.Cells["A2"].PutValue("Option 2");
            worksheet.Cells["A3"].PutValue("Option 3");

            // Bağlantılı hücreden seçili değeri güncelle
            worksheet.Cells["B1"].PutValue("Option 2");
            worksheet.Shapes.UpdateSelectedValue();

            // Value özelliğini almayı göster
            Console.WriteLine("ComboBox Value: " + comboBox.Value);

            // Çalışma kitabını kaydedin
            workbook.Save("ComboBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


