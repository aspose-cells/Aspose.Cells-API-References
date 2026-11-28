---
title: "Cells.CopyRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir bütün satırın veri ve biçimlerini kopyalar"
type: docs
url: /tr/net/aspose.cells/cells/copyrow/
---
## Cells.CopyRow method

Bir bütün satırın veri ve biçimlerini kopyalar.

```csharp
public void CopyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells | Hücreler | Kaynak Cells nesnesi, kopyalanacak veri ve biçimleri içerir. |
| sourceRowIndex | Int32 | Kaynak satır indeksi. |
| destinationRowIndex | Int32 | Hedef satır indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyRowWithCellsInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet1 = workbook.Worksheets[0];
            Cells cells1 = worksheet1.Cells;
            
            // İlk satıra bazı veriler ekle
            cells1["A1"].PutValue("Source Data");
            cells1["B1"].PutValue(100);
            cells1["C1"].PutValue(DateTime.Now);
            
            // İkinci çalışma sayfasını oluştur
            Worksheet worksheet2 = workbook.Worksheets.Add("Sheet2");
            Cells cells2 = worksheet2.Cells;
            
            // Satırı Sheet1'den Sheet2'ye kopyala
            cells2.CopyRow(cells1, 0, 0);
            
            // Satırı Sheet1 içinde yeni konumlara kopyala
            cells1.CopyRow(cells1, 0, 1);
            cells1.CopyRow(cells1, 0, 2);
            
            // Çalışma kitabını kaydedin
            workbook.Save("CopyRowExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


