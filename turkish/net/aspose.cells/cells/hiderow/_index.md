---
title: "Cells.HideRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir satırı gizler"
type: docs
url: /tr/net/aspose.cells/cells/hiderow/
---
## Cells.HideRow method

Bir satırı gizler.

```csharp
public void HideRow(int row)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideRowWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Satır 5'i gizle
            worksheet.Cells.HideRow(5);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


