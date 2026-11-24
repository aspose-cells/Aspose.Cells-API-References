---
title: "Enum TxtValueQuoteType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.TxtValueQuoteType-Enum. Gibt den Typ der Verwendung von Anführungszeichen für Werte in Textformatdateien an."
type: docs
url: /de/net/aspose.cells/txtvaluequotetype/
---
## TxtValueQuoteType enumeration

Gibt den Typ der Verwendung von Anführungszeichen für Werte in Textformatdateien an.

```csharp
public enum TxtValueQuoteType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Normal | `0` | Alle Werte, die Sonderzeichen wie Anführungszeichen oder Trennzeichen enthalten, werden in Anführungszeichen gesetzt. Entspricht dem Verhalten von MS Excel beim Exportieren von Textdateien. |
| Always | `1` | Alle Werte werden immer in Anführungszeichen gesetzt. |
| Minimum | `2` | Werte werden nur bei Bedarf in Anführungszeichen gesetzt. Zum Beispiel, wenn ein Wert Anführungszeichen enthält, diese aber nicht am Anfang des Wertes stehen, wird der Wert nicht in Anführungszeichen gesetzt. |
| Never | `3` | Alle Werte werden nicht in Anführungszeichen gesetzt. Die exportierte Textdatei dieses Typs kann möglicherweise nicht korrekt wieder eingelesen werden, weil die erforderlichen Anführungszeichen fehlen. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class TxtValueQuoteTypeDemo
    {
        public static void TxtValueQuoteTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells[0, 0].Value = "Name";
            worksheet.Cells[0, 1].Value = "Age";
            worksheet.Cells[1, 0].Value = "John Doe";
            worksheet.Cells[1, 1].Value = 30;
            worksheet.Cells[2, 0].Value = "Jane Smith";
            worksheet.Cells[2, 1].Value = 25;

            // Erstelle TxtSaveOptions und setze den QuoteType
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.QuoteType = TxtValueQuoteType.Always;

            // Speichere die Arbeitsmappe als Textdatei mit dem angegebenen Anführungszeichen-Typ
            workbook.Save("TxtValueQuoteTypeExample.txt", saveOptions);

            Console.WriteLine("Workbook saved with TxtValueQuoteType.Always");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


