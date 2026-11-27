---
title: "Range.AutoFill"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metoden. Fyll automatiskt målområdet"
type: docs
url: /sv/net/aspose.cells/range/autofill/
---
## AutoFill(Range) {#autofill}

Fyller automatiskt målområdet.

```csharp
public void AutoFill(Range target)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | Range | målområdet. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodAutoFillWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["A1"].PutValue(1);
            cells["A2"].PutValue(2);
            
            Aspose.Cells.Range source = cells.CreateRange("A1:A2");
            Aspose.Cells.Range target = cells.CreateRange("A3:A10");
            
            source.AutoFill(target);
            
            workbook.Save("AutoFillWithRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFill(Range, AutoFillType) {#autofill_1}

Fyller automatiskt målområdet.

```csharp
public void AutoFill(Range target, AutoFillType autoFillType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | Range | Det målområdet. |
| autoFillType | AutoFillType | Den automatiska fyllningstypen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodAutoFillWithRangeAutoFillTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1:A5");
            for (int i = 0; i < 5; i++)
            {
                sourceRange[i, 0].PutValue(i + 1);
            }

            Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:B5");
            sourceRange.AutoFill(targetRange, AutoFillType.Series);

            // Verifiera resultatet genom att skriva ut värdena
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Target cell B{i+1} value: {targetRange[i, 0].IntValue}");
            }
        }
    }
}
```

### Se även

* enum [AutoFillType](../../autofilltype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


