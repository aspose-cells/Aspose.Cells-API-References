---
title: "Klassen PasteOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.PasteOptions-klass. Representerar specialklistringsalternativen"
type: docs
url: /sv/net/aspose.cells/pasteoptions/
---
## PasteOptions class

Representerar alternativ för Klistra in special.

```csharp
public class PasteOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [PasteOptions](pasteoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [IgnoreLinksToOriginalFile](../../aspose.cells/pasteoptions/ignorelinkstooriginalfile/) { get; set; } | Ignorera länkar till originalfilen. |
| [KeepOldTables](../../aspose.cells/pasteoptions/keepoldtables/) { get; set; } | Behåller tabellerna i målintervallet. |
| [OnlyVisibleCells](../../aspose.cells/pasteoptions/onlyvisiblecells/) { get; set; } | Sant betyder att endast synliga celler kopieras. |
| [OperationType](../../aspose.cells/pasteoptions/operationtype/) { get; set; } | Hämtar och anger operationstypen vid inklistring av intervallet. |
| [PasteType](../../aspose.cells/pasteoptions/pastetype/) { get; set; } | Specialklistringstypen. |
| [ShiftFormulasOfShapes](../../aspose.cells/pasteoptions/shiftformulasofshapes/) { get; set; } | Anger om formlerna i formerna ska förskjutas vid kopiering av områden. |
| [SkipBlanks](../../aspose.cells/pasteoptions/skipblanks/) { get; set; } | Anger om tomma celler ska hoppas över. |
| [Transpose](../../aspose.cells/pasteoptions/transpose/) { get; set; } | Sant för att transponera rader och kolumner när området klistras in. Standardvärdet är Falskt. |

### Exempel

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsDemo
    {
        public static void PasteOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till lite data i det första kalkylbladet
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");
            sheet.Cells["A3"].PutValue(123);

            // Skapa ett annat kalkylblad
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");

            // Definiera källintervallet
            Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange("A1:A3");

            // Definiera destinationsintervallet
            Aspose.Cells.Range destRange = sheet2.Cells.CreateRange("B1:B3");

            // Skapa ett PasteOptions-objekt
            PasteOptions pasteOptions = new PasteOptions
            {
                PasteType = PasteType.Values,
                SkipBlanks = true,
                OnlyVisibleCells = false,
                Transpose = false,
                OperationType = PasteOperationType.None,
                IgnoreLinksToOriginalFile = true
            };

            // Kopiera området med de angivna inklistringsalternativen
            destRange.Copy(sourceRange, pasteOptions);

            // Spara arbetsboken
            workbook.Save("PasteOptionsExample.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


