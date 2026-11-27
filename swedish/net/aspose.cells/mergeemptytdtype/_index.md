---
title: "Enum MergeEmptyTdType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.MergeEmptyTdType enum. Representerar sammanslagningstypen för ett tomt TD-element när en fil exporteras till HTML"
type: docs
url: /sv/net/aspose.cells/mergeemptytdtype/
---
## MergeEmptyTdType enumeration

Representerar sammanslagningstypen för ett tomt TD-element vid export av en fil till HTML.

```csharp
public enum MergeEmptyTdType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Default | `0` | Visa som MS Excel. |
| None | `1` | Tomma TD-element kommer inte att slås ihop när filen exporteras till HTML. Detta kommer att generera en avsevärt större HTML-fil. |
| MergeForcely | `2` | Tvingad sammanslagning av tomt TD-element när filen exporteras till HTML. Storleken på HTML-filen kommer att minskas avsevärt efter att värdet satts till true. Om du vill importera HTML-filen till Excel eller exportera perfekta rutnätslinjer när du sparar filen till HTML, behåll standardvärdet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MergeEmptyTdTypeDemo
    {
        public static void MergeEmptyTdTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Data1");
            worksheet.Cells["B1"].PutValue("Data2");
            worksheet.Cells["C1"].PutValue("Data3");

            // Skapa HtmlSaveOptions och ange egenskapen MergeEmptyTdType
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.MergeEmptyTdType = MergeEmptyTdType.MergeForcely;

            // Spara arbetsboken i HTML-format
            workbook.Save("MergeEmptyTdTypeExample.html", saveOptions);

            Console.WriteLine("HTML file saved with MergeEmptyTdType.MergeForcely option.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


