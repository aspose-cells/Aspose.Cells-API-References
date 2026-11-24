---
title: "Range.AutoFill"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Füllt den Zielbereich automatisch aus"
type: docs
url: /de/net/aspose.cells/range/autofill/
---
## AutoFill(Range) {#autofill}

Füllt den Zielbereich automatisch aus.

```csharp
public void AutoFill(Range target)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ziel | Range | den Zielbereich. |

### Beispiele

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

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFill(Range, AutoFillType) {#autofill_1}

Füllt den Zielbereich automatisch aus.

```csharp
public void AutoFill(Range target, AutoFillType autoFillType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ziel | Range | Der Zielbereich. |
| autoFillType | AutoFillType | Der Auto-Fill-Typ. |

### Beispiele

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

            // Überprüfen Sie das Ergebnis, indem Sie Werte ausgeben
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Target cell B{i+1} value: {targetRange[i, 0].IntValue}");
            }
        }
    }
}
```

### Siehe auch

* enum [AutoFillType](../../autofilltype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


