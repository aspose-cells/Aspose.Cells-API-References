---
title: "Klass DeleteBlankOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DeleteBlankOptions-klass. Representerar inställningen för att ta bort tomma celler/rader/kolumner"
type: docs
url: /sv/net/aspose.cells/deleteblankoptions/
---
## DeleteBlankOptions class

Representerar inställningen för att ta bort tomma celler/rader/kolumner.

```csharp
public class DeleteBlankOptions : DeleteOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [DeleteBlankOptions](deleteblankoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [DrawingsAsBlank](../../aspose.cells/deleteblankoptions/drawingsasblank/) { get; set; } | Anger om ritningsrelaterade objekt såsom bild, form, diagram... ska betraktas som tomma. Standardvärdet är true. |
| [EmptyFormulaValueAsBlank](../../aspose.cells/deleteblankoptions/emptyformulavalueasblank/) { get; set; } | Om en cell ska betraktas som tom när den är en formel och det beräknade resultatet är null eller en tom sträng. Standardvärdet är false. |
| [EmptyStringAsBlank](../../aspose.cells/deleteblankoptions/emptystringasblank/) { get; set; } | Anger om en cell ska betraktas som tom när dess värde är en tom sträng. Standardvärdet är true. |
| [EndIndex](../../aspose.cells/deleteblankoptions/endindex/) { get; set; } | Specificerar slutrad-/kolumnindex (inklusive) för området som ska kontrolleras och där tomma rader/kolumner tas bort. Standardvärdet är -1 och -1 betyder det maximala intervallet för alla objekt (celler, ritningar, ...) som måste kontrolleras. |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | Hämtar/ställer in övervakaren för att spåra förändringar som orsakas av raderingen.(Ärvd från [`DeleteOptions`](../deleteoptions/).) |
| [MergedCellsShrinkType](../../aspose.cells/deleteblankoptions/mergedcellsshrinktype/) { get; set; } | Anger hur sammanslagna celler ska behandlas när tomma rader/kolumner tas bort. |
| [StartIndex](../../aspose.cells/deleteblankoptions/startindex/) { get; set; } | Specificerar startrad-/kolumnindex för området som ska kontrolleras och där tom rad/kolumn tas bort. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | Anger om referenser i andra arbetsblad ska uppdateras.(Ärvd från [`DeleteOptions`](../deleteoptions/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DeleteBlankOptionsDemo
    {
        public static void DeleteBlankOptionsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i arbetsbladet med några data
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

            // Skapa en instans av DeleteBlankOptions
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true,
                EmptyFormulaValueAsBlank = false,
                UpdateReference = true
            };

            // Ta bort tomma rader baserat på alternativen
            worksheet.Cells.DeleteBlankRows(options);

            // Spara arbetsboken
            workbook.Save("DeleteBlankOptionsExample.xlsx");
            workbook.Save("DeleteBlankOptionsExample.pdf");
            return;
        }
    }
}
```

### Se även

* class [DeleteOptions](../deleteoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


