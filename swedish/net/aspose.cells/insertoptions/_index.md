---
title: "Klass InsertOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.InsertOptions-klass. Representerar alternativen för infogning"
type: docs
url: /sv/net/aspose.cells/insertoptions/
---
## InsertOptions class

Representerar alternativen för infogning.

```csharp
public class InsertOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [InsertOptions](insertoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CopyFormatType](../../aspose.cells/insertoptions/copyformattype/) { get; set; } |  |
| [FormulaChangeMonitor](../../aspose.cells/insertoptions/formulachangemonitor/) { get; set; } | Hämtar/anger övervakaren för att spåra ändringar som orsakas av infogningen. |
| [UpdateReference](../../aspose.cells/insertoptions/updatereference/) { get; set; } | Anger om referenser i andra kalkylblad kommer att uppdateras. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InsertOptionsDemo
    {
        public static void InsertOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av InsertOptions
            InsertOptions insertOptions = new InsertOptions
            {
                CopyFormatType = CopyFormatType.SameAsAbove,
                UpdateReference = true
            };

            // Definiera cellområdet där rader kommer att infogas
            CellArea cellArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };

            // Infoga rader med de angivna alternativen
            worksheet.Cells.InsertRows(5, 3, insertOptions);

            // Spara arbetsboken
            workbook.Save("InsertOptionsExample.xlsx");
            workbook.Save("InsertOptionsExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


