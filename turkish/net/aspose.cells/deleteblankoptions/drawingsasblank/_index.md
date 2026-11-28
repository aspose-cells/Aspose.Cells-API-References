---
title: "DeleteBlankOptions.DrawingsAsBlank"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DeleteBlankOptions özelliği. Resim, şekil, grafik... gibi çizimle ilgili nesnelerin boş kabul edilip edilmeyeceğini gösterir. Varsayılan değer true'tir."
type: docs
url: /tr/net/aspose.cells/deleteblankoptions/drawingsasblank/
---
## DeleteBlankOptions.DrawingsAsBlank property

Resim, şekil, grafik gibi çizimle ilgili nesnelerin boş kabul edilip edilmeyeceğini gösterir. Varsayılan değer doğrudur.

```csharp
public bool DrawingsAsBlank { get; set; }
```

### Açıklamalar

Bu özellik false olarak ayarlandığında, çizim nesneleri tarafından kapsanan tüm satır/sütunlar boş kabul edilmez ve silinmez.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyDrawingsAsBlankDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data");
            worksheet.Cells["B1"].PutValue("");
            worksheet.Cells["B2"].PutValue("");

            // DrawingsAsBlank davranışını test etmek için bir çizim nesnesi ekle
            worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);

            // DrawingsAsBlank = false ile boş sütunları sil (çizimleri korur)
            worksheet.Cells.DeleteBlankColumns(new DeleteBlankOptions { DrawingsAsBlank = false });

            Console.WriteLine("Drawing preserved count: " + worksheet.Shapes.Count);
        }
    }
}
```

### Ayrıca Bakınız

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


