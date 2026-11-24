---
title: "Aufzählung PrintErrorsType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.PrintErrorsType enum. Stellt Konstanten für Druckfehler dar"
type: docs
url: /de/net/aspose.cells/printerrorstype/
---
## PrintErrorsType enumeration

Stellt Druckfehlerkonstanten dar.

```csharp
public enum PrintErrorsType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| PrintErrorsBlank | `0` | Stellt dar, dass Fehler nicht gedruckt werden. |
| PrintErrorsDash | `1` | Stellt dar, dass Fehler als "--" gedruckt werden. |
| PrintErrorsDisplayed | `2` | Stellt dar, dass Fehler wie angezeigt gedruckt werden. |
| PrintErrorsNA | `3` | Stellt dar, dass Fehler als "#N/A" gedruckt werden. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintErrorsTypeDemo
    {
        public static void PrintErrorsTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf die Seiteneinrichtung des Arbeitsblatts
            PageSetup pageSetup = worksheet.PageSetup;

            // Verschiedene Druckfehlertypen festlegen
            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
            workbook.Save("PrintErrorsBlank.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
            workbook.Save("PrintErrorsDash.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsDisplayed;
            workbook.Save("PrintErrorsDisplayed.xlsx");

            pageSetup.PrintErrors = PrintErrorsType.PrintErrorsNA;
            workbook.Save("PrintErrorsNA.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


