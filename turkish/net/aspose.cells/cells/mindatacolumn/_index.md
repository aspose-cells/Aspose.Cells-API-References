---
title: "Cells.MinDataColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Veri içeren hücrenin minimum sütun indeksi"
type: docs
url: /tr/net/aspose.cells/cells/mindatacolumn/
---
## Cells.MinDataColumn property

Veri içeren hücrenin minimum sütun indeksi.

```csharp
public int MinDataColumn { get; }
```

### Açıklamalar

-1 will be returned if there is no cell which contains data. This property needs to iterate and check all cells in a worksheet dynamically, so it is a time-consumed progress and should not be invoked repeatedly, such as using it directly as condition in a loop.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinDataColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Hücrelere bazı veriler ekle (sütun 2'den başlayarak)
            cells["B1"].PutValue("Header1");
            cells["C2"].PutValue("Data1");
            cells["D3"].PutValue("Data2");
            cells["E4"].PutValue("Data3");
            
            // Veri içeren minimum sütun indeksini alın.
            int minDataColumn = cells.MinDataColumn;
            
            // Sonucu çıktı olarak ver
            Console.WriteLine("Minimum data column index: " + minDataColumn);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


