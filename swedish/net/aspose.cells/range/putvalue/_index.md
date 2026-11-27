---
title: "Range.PutValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metod. Sätter ett värde i området; om lämpligt kommer värdet att konverteras till en annan datatyp och cellernas talformat återställas"
type: docs
url: /sv/net/aspose.cells/range/putvalue/
---
## Range.PutValue method

Sätter ett värde i området, om lämpligt konverteras värdet till en annan datatyp och cellens talformat återställs.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stringValue | String | Ange värde |
| isConverted | Boolean | True: konverterad till annan datatyp om lämpligt. |
| setStyle | Boolean | True: sätt talformatet till cellens stil vid konvertering till annan datatyp |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1:B10");
            range.PutValue("123", true, false);
            
            Console.WriteLine("Value at A5: " + cells["A5"].DoubleValue);
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


