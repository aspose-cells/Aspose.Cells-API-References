---
title: "ComboBoxActiveXControl.IsAutoWordSelected"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ComboBoxActiveXControl özelliği. Seçimi genişletmek için kullanılan temel birimi belirtir. True, temel birimin tek bir karakter olduğunu belirtir. false, temel birimin bütün bir kelime olduğunu belirtir"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/isautowordselected/
---
## ComboBoxActiveXControl.IsAutoWordSelected property

Bir seçimi genişletmek için kullanılan temel birimi belirtir. True, temel birimin tek bir karakter olduğunu belirtir. false, temel birimin tam bir kelime olduğunu belirtir.

```csharp
public virtual bool IsAutoWordSelected { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyIsAutoWordSelectedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tüm gerekli parametrelerle bir ComboBox ActiveX kontrolü ekle
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 100, 20, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Temel özellikleri yapılandırın
            comboBox.ListRows = 5;
            comboBox.ColumnCount = 1;
            comboBox.Value = "Sample Text";

            // IsAutoWordSelected özelliğini göster
            comboBox.IsAutoWordSelected = false;
            Console.WriteLine("IsAutoWordSelected set to: " + comboBox.IsAutoWordSelected);

            // Çalışma kitabını kaydedin
            workbook.Save("ComboBoxIsAutoWordSelectedDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


