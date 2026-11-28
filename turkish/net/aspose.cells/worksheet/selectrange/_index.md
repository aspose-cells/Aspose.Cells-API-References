---
title: "Worksheet.SelectRange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Bir aralığı seçer"
type: docs
url: /tr/net/aspose.cells/worksheet/selectrange/
---
## Worksheet.SelectRange method

Bir aralığı seçer.

```csharp
public void SelectRange(int startRow, int startColumn, int totalRows, int totalColumns, 
    bool removeOthers)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Başlangıç satırı. |
| startColumn | Int32 | Başlangıç sütunu |
| totalRows | Int32 | Satır sayısı. |
| totalColumns | Int32 | Sütun sayısı |
| removeOthers | Boolean | True, diğer seçili aralıkları kaldırıp yalnızca bu aralığı seçmek anlamına gelir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSelectRangeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Satır 1, sütun 1'den satır 5, sütun 5'e (B2:F6) kadar aralığı seç ve etkinleştir
            worksheet.SelectRange(1, 1, 5, 5, true);
            
            Console.WriteLine("Active cell: " + worksheet.ActiveCell);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


