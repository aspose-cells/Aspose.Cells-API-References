---
title: "ListBox.Shadow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListBox özelliği. Combo kutusunun 3D gölgelendirmeye sahip olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing/listbox/shadow/
---
## ListBox.Shadow property

ComboBox'ın 3D gölgelendirmeye sahip olup olmadığını gösterir.

```csharp
public bool Shadow { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertyShadowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Liste öğelerini doldur
            worksheet.Cells["A1"].PutValue("Option 1");
            worksheet.Cells["A2"].PutValue("Option 2");
            worksheet.Cells["A3"].PutValue("Option 3");

            // Liste kutusunu oluştur ve temel özellikleri ayarla
            ListBox listBox = worksheet.Shapes.AddListBox(2, 1, 5, 1, 100, 150);
            listBox.InputRange = "A1:A3";
            listBox.LinkedCell = "B1";
            
            // Gölge özelliğini ayarla
            listBox.Shadow = true;

            // Doğrulamak için kaydedin ve yeniden yükleyin
            workbook.Save("ListBoxShadowDemo.xlsx");
            
            Workbook loadedWorkbook = new Workbook("ListBoxShadowDemo.xlsx");
            ListBox loadedBox = (ListBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            Console.WriteLine("Shadow enabled: " + loadedBox.Shadow);
        }
    }
}
```

### Ayrıca Bakınız

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


