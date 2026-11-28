---
title: "PasteOptions.OnlyVisibleCells"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PasteOptions özelliği. True, yalnızca görünen hücrelerin kopyalanması anlamına gelir"
type: docs
url: /tr/net/aspose.cells/pasteoptions/onlyvisiblecells/
---
## PasteOptions.OnlyVisibleCells property

True, yalnızca görünen hücrelerin kopyalanması anlamına gelir.

```csharp
public bool OnlyVisibleCells { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyOnlyVisibleCellsDemo
    {
        public static void Run()
        {
            // İki çalışma sayfası içeren bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // İlk çalışma sayfasından hücreleri al ve verileri doldur
            Cells sourceCells = workbook.Worksheets[0].Cells;
            sourceCells["A1"].PutValue("Hidden A1");
            sourceCells["B2"].PutValue("Visible B2");
            sourceCells["C3"].PutValue("Hidden C3");
            
            // Bazı satır ve sütunları gizle
            sourceCells.HideRow(0);  // Hides row 1 (A1)
            sourceCells.HideColumn(2); // Hides column C (C3)

            // Kopyalamak için kaynak aralığı oluştur
            Aspose.Cells.Range sourceRange = sourceCells.CreateRange("A1:C3");
            
            // Hedef için ikinci çalışma sayfasından hücreleri al
            Cells destCells = workbook.Worksheets[1].Cells;
            Aspose.Cells.Range destRange = destCells.CreateRange("A1:C3");
            
            // Yapıştırma seçenekleri oluştur ve OnlyVisibleCells'i ayarla
            PasteOptions pasteOptions = new PasteOptions();
            pasteOptions.OnlyVisibleCells = true;
            
            // Yalnızca görünen hücreleri kopyala
            destRange.Copy(sourceRange, pasteOptions);
            
            // İşlevselliği göstermek için sonuçları çıktı al
            Console.WriteLine("B2 value (should be copied): " + destCells["B2"].StringValue);
            Console.WriteLine("A1 value (should be empty): " + destCells["A1"].StringValue);
            Console.WriteLine("C3 value (should be empty): " + destCells["C3"].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


