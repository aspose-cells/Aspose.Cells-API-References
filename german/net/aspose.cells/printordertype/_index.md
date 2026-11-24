---
title: "Enum PrintOrderType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.PrintOrderType Enum. Stellt Druckreihenfolge-Konstanten dar"
type: docs
url: /de/net/aspose.cells/printordertype/
---
## PrintOrderType enumeration

Stellt Druckreihenfolgekonstanten dar.

```csharp
public enum PrintOrderType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| DownThenOver | `0` | Nach unten, dann nach rechts |
| OverThenDown | `1` | Nach rechts, dann nach unten |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintOrderTypeDemo
    {
        public static void PrintOrderTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greifen Sie auf das PageSetup-Objekt zu
            PageSetup pageSetup = worksheet.PageSetup;

            // Setzen Sie die Druckreihenfolge auf DownThenOver
            pageSetup.Order = PrintOrderType.DownThenOver;

            // Setzen Sie einige weitere PageSetup-Eigenschaften zum Demonstrationszweck.
            pageSetup.PrintArea = "A1:D10";
            pageSetup.PrintTitleRows = "$1:$1";
            pageSetup.PrintTitleColumns = "$A:$A";
            pageSetup.CenterHorizontally = true;
            pageSetup.CenterVertically = true;

            // Speichere die Arbeitsmappe
            workbook.Save("PrintOrderTypeExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


