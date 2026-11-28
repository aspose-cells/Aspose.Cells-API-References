---
title: "ComboBox.SelectedValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ComboBox özelliği. Combo kutusunun seçili değerini alır"
type: docs
url: /tr/net/aspose.cells.drawing/combobox/selectedvalue/
---
## ComboBox.SelectedValue property

Combo kutusunun seçili değerini alır.

```csharp
public string SelectedValue { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertySelectedValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir ComboBox oluşturun ve öğeler ekleyin
            Aspose.Cells.Drawing.ComboBox comboBox = (Aspose.Cells.Drawing.ComboBox)worksheet.Shapes.AddComboBox(1, 0, 1, 0, 100, 50);
            comboBox.LinkedCell = "A1";
            comboBox.SetInputRange("B1:B4", false, false);
            
            // Giriş aralığındaki değerleri ayarlayın
            worksheet.Cells["B1"].PutValue("a");
            worksheet.Cells["B2"].PutValue("b");
            worksheet.Cells["B3"].PutValue("c");
            worksheet.Cells["B4"].PutValue("d");

            // SelectedValue'ı (yalnızca okuma özelliği) gösterin
            Console.WriteLine("SelectedValue: " + comboBox.SelectedValue);

            // Çalışma kitabını kaydedin
            workbook.Save("ComboBoxDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


