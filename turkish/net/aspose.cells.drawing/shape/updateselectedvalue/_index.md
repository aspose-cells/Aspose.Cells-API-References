---
title: "Shape.UpdateSelectedValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Shape yöntemi. Seçili değeri bağlı hücrenin değeriyle güncelleyin"
type: docs
url: /tr/net/aspose.cells.drawing/shape/updateselectedvalue/
---
## Shape.UpdateSelectedValue method

Seçili değeri, bağlı hücrenin değeriyle günceller.

```csharp
public void UpdateSelectedValue()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodUpdateSelectedValueDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Biraz örnek veri doldurun
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;
            }

            // Bir ListBox şekli oluşturun
            Shape listBoxShape = worksheet.Shapes.AddListBox(2, 0, 2, 0, 130, 130);
            
            // Giriş aralığını ve bağlı hücreyi ayarlayın
            listBoxShape.SetInputRange("$A$1:$A$6", false, false);
            listBoxShape.SetLinkedCell("$A$12", false, true);

            // ListBox nesnesini alın
            ListBox listBox = (ListBox)listBoxShape;

            // Bağlı hücrede başlangıç değerini ayarlayın ve seçimi güncelleyin
            worksheet.Cells["A12"].Value = 3;
            listBoxShape.UpdateSelectedValue();

            // Seçimi doğrulayın
            if (listBox.IsSelected(2))
            {
                Console.WriteLine("Option 3 is selected");
            }

            // Değeri değiştirin ve seçimi tekrar güncelleyin
            worksheet.Cells["A12"].Value = 4;
            listBoxShape.UpdateSelectedValue();

            if (listBox.IsSelected(3))
            {
                Console.WriteLine("Option 4 is selected");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


