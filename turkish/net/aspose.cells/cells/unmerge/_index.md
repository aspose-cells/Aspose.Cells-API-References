---
title: "Cells.UnMerge"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells metodu. Belirtilen birleştirilmiş hücre aralığının birleştirmesini kaldırır"
type: docs
url: /tr/net/aspose.cells/cells/unmerge/
---
## Cells.UnMerge method

Belirtilen birleştirilmiş hücre aralığının birleştirmesini kaldırır.

```csharp
public void UnMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | Int32 | Bu aralığın ilk satırı (sıfır tabanlı) |
| firstColumn | Int32 | Bu aralığın ilk sütunu (sıfır tabanlı) |
| totalRows | Int32 | Satır sayısı (bir tabanlı) |
| totalColumns | Int32 | Sütun sayısı (bir tabanlı) |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnMergeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Önce hücreleri birleştirin
            cells.Merge(0, 0, 2, 2);
            
            // Daha önce birleştirilmiş hücrelerin birleştirmesini kaldırın
            cells.UnMerge(0, 0, 2, 2);
            
            // Çalışma kitabını kaydedin
            workbook.Save("UnMergeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


