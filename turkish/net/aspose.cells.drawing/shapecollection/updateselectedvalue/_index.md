---
title: "ShapeCollection.UpdateSelectedValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapeCollection yöntemi. Bağlı hücre veya şeklin aralığının değeriyle seçili değeri günceller"
type: docs
url: /tr/net/aspose.cells.drawing/shapecollection/updateselectedvalue/
---
## ShapeCollection.UpdateSelectedValue method

Seçili değeri, şeklin bağlı hücresi veya aralığının değeriyle güncelle.

```csharp
public void UpdateSelectedValue()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodUpdateSelectedValueDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bir şekil (açılır liste) ekleyin
            Aspose.Cells.Drawing.ListBox listBox = (Aspose.Cells.Drawing.ListBox)worksheet.Shapes.AddListBox(0, 0, 100, 100, 3, 20);
            
            // Liste öğelerini ve seçili değeri ayarlayın
            listBox.SetInputRange("A1:A3", false, false);
            listBox.SelectedIndex = 1;
            
            // Şekildeki seçili değeri güncelleyin
            worksheet.Shapes.UpdateSelectedValue();
            
            // Çalışma kitabını kaydedin
            workbook.Save("ShapeCollectionUpdateSelectedValueDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


