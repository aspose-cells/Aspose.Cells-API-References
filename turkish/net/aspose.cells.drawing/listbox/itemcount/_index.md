---
title: "ListBox.ItemCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListBox özelliği. Liste kutusundaki öğe sayısını alır"
type: docs
url: /tr/net/aspose.cells.drawing/listbox/itemcount/
---
## ListBox.ItemCount property

Liste kutusundaki öğe sayısını alır.

```csharp
public int ItemCount { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListBoxPropertyItemCountDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("Sheet1");

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Mango");

            // Liste kutusunu oluştur ve özellikleri ayarla
            Aspose.Cells.Drawing.ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 10, 0, 100, 150);
            listBox.InputRange = "A1:A4";
            
            // ItemCount kullanımını göster
            int itemCount = listBox.ItemCount;
            Console.WriteLine("ListBox contains {0} items", itemCount);
            
            // Öğe sayısına göre listbox yüksekliğini ayarla
            listBox.Height = itemCount * 15;

            workbook.Save("ListBoxItemCountDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


