---
title: "Cell.SharedStyleIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Hücrenin stil havuzundaki paylaşılan stil dizinini alır"
type: docs
url: /tr/net/aspose.cells/cell/sharedstyleindex/
---
## Cell.SharedStyleIndex property

Stil havuzundaki hücrenin paylaşılan stil indeksini alır.

```csharp
public int SharedStyleIndex { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertySharedStyleIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir stil oluştur ve bazı özellikleri ayarla
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;

            // Stili A1 hücresine uygula
            worksheet.Cells["A1"].SetStyle(style);

            // A1 hücresinin paylaşılan stil dizinini al
            int sharedStyleIndex = worksheet.Cells["A1"].SharedStyleIndex;

            // Dizini kullanarak stil havuzundan stili al
            Style retrievedStyle = workbook.GetStyleInPool(sharedStyleIndex);

            // Stil bilgilerini doğrulamak için çıktıya gönder
            Console.WriteLine("Font Name: " + retrievedStyle.Font.Name);
            Console.WriteLine("Font Size: " + retrievedStyle.Font.Size);
            Console.WriteLine("Is Bold: " + retrievedStyle.Font.IsBold);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


