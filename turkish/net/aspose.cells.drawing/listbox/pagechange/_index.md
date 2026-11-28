---
title: "ListBox.PageChange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListBox özelliği. Kullanıcı kaydırma çubuklarının sayfa yukarı veya sayfa aşağı bölgesine tıkladığında kontrolün değerinin değiştiği miktarı belirtir"
type: docs
url: /tr/net/aspose.cells.drawing/listbox/pagechange/
---
## ListBox.PageChange property

Kullanıcı kaydırma çubuğunun sayfa yukarı veya sayfa aşağı bölgesine tıkladığında kontrolün değerinin değiştirildiği miktarı belirtir.

```csharp
public int PageChange { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertyPageChangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir ListBox şekli ekle
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(1, 0, 1, 0, 100, 100);

            // ListBox için bazı öğeler ayarla
            listBox.SetInputRange("A1:A5", false, false);
            
            // PageChange özelliğini ayarla
            listBox.PageChange = 2;

            // Çalışma kitabını kaydedin
            workbook.Save("ListBoxPageChangeDemo.xlsx");

            // PageChange değerini göster
            Console.WriteLine("ListBox PageChange value: " + listBox.PageChange);
        }
    }
}
```

### Ayrıca Bakınız

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


