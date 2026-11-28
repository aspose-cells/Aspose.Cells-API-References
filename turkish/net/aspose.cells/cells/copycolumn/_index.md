---
title: "Cells.CopyColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir bütün sütunun veri ve biçimlerini kopyalar"
type: docs
url: /tr/net/aspose.cells/cells/copycolumn/
---
## Cells.CopyColumn method

Bir bütün sütunun veri ve biçimlerini kopyalar.

```csharp
public void CopyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceCells | Hücreler | Kaynak Cells nesnesi, kopyalanacak veri ve biçimleri içerir. |
| sourceColumnIndex | Int32 | Kaynak sütun indeksi. |
| destinationColumnIndex | Int32 | Hedef sütun indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCopyColumnWithCellsInt32Int32Demo
    {
        public static void Run()
        {
            // Kaynak çalışma kitabını oluştur ve verileri doldur
            Workbook wbSrc = new Workbook();
            Cells cellsSrc = wbSrc.Worksheets[0].Cells;
            cellsSrc[0, 255].PutValue(1);
            cellsSrc[1, 255].PutValue(true);
            cellsSrc[2, 255].PutValue("abc");
            cellsSrc[3, 255].PutValue(false);
            cellsSrc[65535, 255].PutValue(2.56);

            // Hedef çalışma kitabı oluştur
            Workbook wbDest = new Workbook();
            Cells cellsDest = wbDest.Worksheets[0].Cells;

            // Sütunu kaynaktan hedefe kopyala
            cellsDest.CopyColumn(cellsSrc, 255, 0);

            // Sonucu kaydet
            wbDest.Save("outputCopyColumn.xlsx");
            
            Console.WriteLine("Column copied successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


