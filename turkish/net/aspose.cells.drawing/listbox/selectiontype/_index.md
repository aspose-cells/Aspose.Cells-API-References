---
title: "ListBox.SelectionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListBox özelliği. Belirtilen liste kutusunun seçim modunu alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/listbox/selectiontype/
---
## ListBox.SelectionType property

Belirtilen liste kutusunun seçim modunu alır veya ayarlar.

```csharp
public SelectionType SelectionType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertySelectionTypeDemo
    {
        public static void Run()
        {
            // Yeni bir Workbook oluşturun
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Liste kutusu için örnek veri ekle
            sheet.Cells["A1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Finance");
            sheet.Cells["A3"].PutValue("MIS");
            sheet.Cells["A4"].PutValue("R&D");

            // Bir liste kutusu ekle
            ListBox listBox = sheet.Shapes.AddListBox(1, 0, 2, 0, 100, 80);
            
            // Liste kutusu özelliklerini ayarla
            listBox.InputRange = "A1:A4";
            listBox.LinkedCell = "B1";
            
            // SelectionType özelliğini göster
            listBox.SelectionType = SelectionType.Single; // Only single selection allowed
            listBox.SelectedIndex = 1; // Select "Finance"

            // Çalışma kitabını kaydedin
            workbook.Save("ListBoxSelectionTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SelectionType](../../selectiontype/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


