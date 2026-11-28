---
title: "ComboBox.DropDownLines"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ComboBox özelliği. Bir combo kutusunun açılır bölümünde görüntülenen liste satır sayısını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/combobox/dropdownlines/
---
## ComboBox.DropDownLines property

Bir combo kutusunun açılır bölümünde gösterilen liste satırı sayısını alır veya ayarlar.

```csharp
public int DropDownLines { get; set; }
```

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertyDropDownLinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir ComboBox oluşturun
            ComboBox comboBox = worksheet.Shapes.AddComboBox(0, 0, 0, 0, 100, 100);
            comboBox.DropDownLines = 5;
            
            // Çalışma sayfası hücrelerini öğelerle doldurun
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");
            worksheet.Cells["A6"].PutValue("Item 6");

            // Combo kutusunu hücre değerlerine bağlayın
            comboBox.InputRange = "A1:A6";

            workbook.Save("ComboBoxDropDownLinesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


