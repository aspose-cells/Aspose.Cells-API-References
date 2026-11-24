---
title: "Cell.HasCustomStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt an, ob diese Zelle benutzerdefinierte Stil-Einstellungen hat, die sich vom Standard unterscheiden, der von der entsprechenden Zeile, Spalte oder Arbeitsmappe geerbt wird."
type: docs
url: /de/net/aspose.cells/cell/hascustomstyle/
---
## Cell.HasCustomStyle property

Gibt an, ob diese Zelle benutzerdefinierte Stileinstellungen hat (anders als die Standard‑Einstellungen, die von der entsprechenden Zeile, Spalte oder Arbeitsmappe geerbt werden).

```csharp
public bool HasCustomStyle { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Check HasCustomStyle");

            // Anfangswert von HasCustomState anzeigen (erbt Standardstil)
            Console.WriteLine("Initial HasCustomStyle: " + cell.HasCustomStyle);

            // Benutzerdefinierten Stil erstellen und auf die Zelle anwenden
            Style customStyle = workbook.CreateStyle();
            customStyle.Font.IsBold = true;
            cell.SetStyle(customStyle);

            // Überprüfen, ob HasCustomStyle nach einer Stiländerung true ist
            Console.WriteLine("After applying custom style - HasCustomStyle: " + cell.HasCustomStyle);

            // Arbeitsmappe mit angewendetem benutzerdefiniertem Stil speichern
            workbook.Save("CellCustomStyleDemo.xlsx");

            // Stil der Zelle auf den Standardstil der Arbeitsmappe zurücksetzen
            Style defaultStyle = workbook.DefaultStyle;
            cell.SetStyle(defaultStyle);

            // Überprüfen Sie, dass HasCustomStyle nach dem Zurücksetzen auf den Standardwert false ist
            Console.WriteLine("After resetting to default style - HasCustomStyle: " + cell.HasCustomStyle);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


