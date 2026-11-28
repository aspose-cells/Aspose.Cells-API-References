---
title: "Cells.IsColumnHidden"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen indeksteki bir sütunun gizli olup olmadığını kontrol eder"
type: docs
url: /tr/net/aspose.cells/cells/iscolumnhidden/
---
## Cells.IsColumnHidden method

Verilen indeksteki sütunun gizli olup olmadığını kontrol eder.

```csharp
public bool IsColumnHidden(int columnIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | Int32 | sütun indeksi |

### Dönüş Değeri

sütun gizli ise doğru.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsColumnHiddenWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // C sütununu gizle (indeks 2)
            cells.HideColumn(2);
            
            // Sütun C'nin gizli olup olmadığını kontrol edin
            bool isHidden = cells.IsColumnHidden(2);
            
            Console.WriteLine("Is column C (index 2) hidden? " + isHidden);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


