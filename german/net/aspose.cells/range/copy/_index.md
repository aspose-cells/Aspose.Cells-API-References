---
title: "Range.Copy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Kopiere den Bereich mit Spezial-Einfügeoptionen"
type: docs
url: /de/net/aspose.cells/range/copy/
---
## Copy(Range, PasteOptions) {#copy_1}

Kopieren des Bereichs mit Spezial‑Einfügeoptionen.

```csharp
public void Copy(Range range, PasteOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Bereich | Range | Der Quellbereich. |
| Optionen | PasteOptions | Die Spezial-Einfügeoptionen. |

### Beispiele

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
            
            // Beispieldaten im Quellbereich erstellen
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Bereiche mit vollständig qualifiziertem Typ erstellen
            Aspose.Cells.Range source = sheet.Cells.CreateRange(0, 0, 5, 5);
            Aspose.Cells.Range destination = sheet.Cells.CreateRange(6, 0, 5, 5);

            // Einfügeoptionen festlegen
            PasteOptions options = new PasteOptions();
            options.PasteType = PasteType.All;

            // Kopieren mit Einfügeoptionen
            destination.Copy(source, options);

            wb.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PasteOptions](../../pasteoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Copy(Range) {#copy}

Kopiert Daten (einschließlich Formeln), Formatierungen, Zeichenobjekte usw. aus einem Quellbereich.

```csharp
public void Copy(Range range)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| range | Range | Quell-[`Range`](../) Objekt. |

### Beispiele

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
            
            // Erstelle Quell- und Zielbereiche
            Aspose.Cells.Range sourceRange = cells.CreateRange("A1:A5");
            Aspose.Cells.Range destRange = cells.CreateRange("A6:A10");
            
            // Quellbereich mit Beispieldaten füllen
            for (int i = 0; i < 5; i++)
            {
                sourceRange[i, 0].PutValue($"Data {i + 1}");
            }
            
            // Quellbereich zum Ziel kopieren
            sourceRange.Copy(destRange);
            
            workbook.Save("RangeCopyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


