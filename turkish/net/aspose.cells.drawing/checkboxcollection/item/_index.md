---
title: "CheckBoxCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CheckBoxCollection özelliği. Belirtilen indeksteki CheckBox öğesini alır"
type: docs
url: /tr/net/aspose.cells.drawing/checkboxcollection/item/
---
## CheckBoxCollection indexer

Belirtilen indeksteki [`CheckBox`](../../checkbox/) öğesini alır.

```csharp
public CheckBox this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Öğenin sıfır tabanlı indeksi. |

### Dönüş Değeri

Belirtilen indeksteki öğe.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bir onay kutusu ekle
            int index = worksheet.CheckBoxes.Add(10, 10, 100, 20);
            
            // Item özelliğini (indeksleyiciyi) kullanarak checkbox'a erişin
            Aspose.Cells.Drawing.CheckBox checkBox = worksheet.CheckBoxes[index];
            checkBox.Text = "Sample CheckBox";
            checkBox.Name = "CheckBox1";
            
            // İndeks (Item özelliği) kullanarak checkbox'a erişin
            Aspose.Cells.Drawing.CheckBox checkBoxByName = worksheet.CheckBoxes[0];
            
            // Checkbox özelliklerini çıktı olarak verin
            Console.WriteLine("CheckBox Name: " + checkBoxByName.Name);
            Console.WriteLine("CheckBox Text: " + checkBoxByName.Text);
            
            // Çalışma kitabını kaydedin
            workbook.Save("CheckBoxExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CheckBox](../../checkbox/)
* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


