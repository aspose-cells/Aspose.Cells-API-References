---
title: "Range.GetOffset"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Ofset ile bir Range aralığını döndürür."
type: docs
url: /tr/net/aspose.cells/range/getoffset/
---
## Range.GetOffset method

Ofset ile [`Range`](../) aralığını alır.

```csharp
public Range GetOffset(int rowOffset, int columnOffset)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowOffset | Int32 | Bu aralıktaki satır ofseti, sıfır tabanlı. |
| columnOffset | Int32 | Bu aralıktaki sütun ofseti, sıfır tabanlı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetOffsetWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // İlk aralığı oluşturun
            Aspose.Cells.Range originalRange = cells.CreateRange("A1");
            Console.WriteLine("Original Range Address: " + originalRange.Address);
            
            // Ofset aralığını alın
            Aspose.Cells.Range offsetRange = originalRange.GetOffset(1, 1);
            Console.WriteLine("Offset Range Address: " + offsetRange.Address);
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


