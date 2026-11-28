---
title: "Cells.IsRowHidden"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen indeksteki bir satırın gizli olup olmadığını kontrol eder"
type: docs
url: /tr/net/aspose.cells/cells/isrowhidden/
---
## Cells.IsRowHidden method

Verilen indeksteki satırın gizli olup olmadığını kontrol eder.

```csharp
public bool IsRowHidden(int rowIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | Int32 | satır indeksi |

### Dönüş Değeri

satır gizli ise true

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsRowHiddenWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Örnek veri
            cells[1, 0].PutValue("US");
            cells[2, 0].PutValue("UK");
            cells[3, 0].PutValue("India");
            cells[4, 0].PutValue("UK");
            cells[5, 0].PutValue("India");
            cells[6, 0].PutValue("US");
            
            // Filtreyi uygula
            AutoFilter af = sheet.AutoFilter;
            af.Range = "A1:A1";
            af.Filter(0, "India");
            af.Refresh();
            
            // Satır görünürlüğünü kontrol et
            Console.WriteLine("Row Visibility Check:");
            for (int i = 1; i < 7; i++)
            {
                Console.WriteLine($"Row {i} hidden: {cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


