---
title: "RadioButton.IsChecked"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RadioButton özelliği. RadioButton'un işaretli olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/radiobutton/ischecked/
---
## RadioButton.IsChecked property

Radyo düğmesinin işaretli olup olmadığını gösterir.

```csharp
public bool IsChecked { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class RadioButtonPropertyIsCheckedDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bir radyo düğmesi ekle
            Shape shape = worksheet.Shapes.AddRadioButton(1, 0, 1, 0, 100, 100);
            RadioButton radioButton = (RadioButton)shape;
            
            // Radyo düğmesinin metnini ayarla
            radioButton.Text = "Option 1";
            
            // Başlangıçta işaretlenmemiş
            radioButton.IsChecked = false;
            Console.WriteLine("Radio button initially unchecked: " + radioButton.IsChecked);
            
            // Radyo düğmesini işaretle
            radioButton.IsChecked = true;
            Console.WriteLine("Radio button after checking: " + radioButton.IsChecked);
            
            // Çalışma kitabını kaydedin
            workbook.Save("RadioButtonExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


