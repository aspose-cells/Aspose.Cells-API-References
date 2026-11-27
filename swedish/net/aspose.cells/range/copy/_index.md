---
title: "Range.Copy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metoden. Kopierar intervallet med specialklistra-alternativ"
type: docs
url: /sv/net/aspose.cells/range/copy/
---
## Copy(Range, PasteOptions) {#copy_1}

Kopierar området med specialklistra in-alternativ.

```csharp
public void Copy(Range range, PasteOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| område | Range | Det källintervallet. |
| alternativ | PasteOptions | De specialklistra-alternativen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyWithRangePasteOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Skapa exempeldata i källintervallet
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Skapa intervall med fullständigt kvalificerad typ
            Aspose.Cells.Range source = sheet.Cells.CreateRange(0, 0, 5, 5);
            Aspose.Cells.Range destination = sheet.Cells.CreateRange(6, 0, 5, 5);

            // Ställ in klistra-alternativ
            PasteOptions options = new PasteOptions();
            options.PasteType = PasteType.All;

            // Kopiera med klistra-alternativ
            destination.Copy(source, options);

            wb.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PasteOptions](../../pasteoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Range) {#copy}

Kopierar data (inklusive formler), formatering, ritobjekt etc. från ett källområde.

```csharp
public void Copy(Range range)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| range | Range | Källa [`Range`](../) objekt. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Skapa käll- och destinationsintervall
            Aspose.Cells.Range sourceRange = cells.CreateRange("A1:A5");
            Aspose.Cells.Range destRange = cells.CreateRange("A6:A10");
            
            // Fyll källintervallet med exempeldata
            for (int i = 0; i < 5; i++)
            {
                sourceRange[i, 0].PutValue($"Data {i + 1}");
            }
            
            // Kopiera källintervallet till destinationen
            sourceRange.Copy(destRange);
            
            workbook.Save("RangeCopyDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


