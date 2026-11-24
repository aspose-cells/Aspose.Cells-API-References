---
title: "TxtSaveOptions.TrimLeadingBlankRowAndColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtSaveOptions-Eigenschaft. Gibt an, ob führende leere Zeilen und Spalten wie in MS Excel entfernt werden sollen. Standard ist true"
type: docs
url: /de/net/aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn/
---
## TxtSaveOptions.TrimLeadingBlankRowAndColumn property

Gibt an, ob führende leere Zeilen und Spalten wie in MS Excel entfernt werden sollen. Standard ist true.

```csharp
public bool TrimLeadingBlankRowAndColumn { get; set; }
```

### Hinweise

Entsprechend der Regel in MS Excel wird eine Zeile/Spalte nicht als leer betrachtet, wenn sie einen benutzerdefinierten Stil hat, selbst wenn sie keine Zellen enthält. Beim Speichern im LightCells-Modus hat diese Option keine Wirkung. Der Benutzer sollte den Ausgabebereich über die Implementierung von [`LightCellsDataProvider`](../lightcellsdataprovider/) oder durch Angabe von [`ExportArea`](../exportarea/) steuern.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyTrimLeadingBlankRowAndColumnDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Beispielarbeitsmappe mit einigen Daten und leeren Zeilen/Spalten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie einige Daten mit führenden leeren Zeilen und Spalten hinzu
            worksheet.Cells["C3"].PutValue("Data1");
            worksheet.Cells["D4"].PutValue("Data2");
            worksheet.Cells["E5"].PutValue("Data3");

            // Speichern ohne führende Leerzeichen zu entfernen
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.TrimLeadingBlankRowAndColumn = false;
            workbook.Save("output_with_blanks.csv", saveOptions);

            // Speichern mit Entfernen führender Leerzeichen
            saveOptions.TrimLeadingBlankRowAndColumn = true;
            workbook.Save("output_trimmed.csv", saveOptions);

            Console.WriteLine("Files saved successfully. Compare output_with_blanks.csv and output_trimmed.csv to see the difference.");
        }
    }
}
```

### Siehe auch

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


