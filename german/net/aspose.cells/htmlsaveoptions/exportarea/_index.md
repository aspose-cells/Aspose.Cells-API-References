---
title: "HtmlSaveOptions.ExportArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions property. Ruft den zu exportierenden CellArea des aktuell aktiven Arbeitsblatts ab oder legt ihn fest. Wenn Sie dieses Attribut setzen, wird der Druckbereich des aktuell aktiven Arbeitsblatts weggelassen. Nur der angegebene Bereich wird beim Speichern der Datei als HTML exportiert."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/exportarea/
---
## HtmlSaveOptions.ExportArea property

Liest oder setzt den zu exportierenden CellArea des aktuell aktiven Worksheet. Wenn Sie dieses Attribut festlegen, wird der Druckbereich des aktuell aktiven Worksheet weggelassen. Nur der angegebene Bereich wird beim Speichern der Datei als html exportiert.

```csharp
public CellArea ExportArea { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportAreaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Daten im Arbeitsblatt einfügen
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell {i},{j}");
                }
            }

            // HTML-Speicheroptionen mit Exportbereich festlegen
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportArea = CellArea.CreateCellArea("B2", "D5");

            // Arbeitsmappe mit angegebenem Exportbereich speichern
            workbook.Save("output.html", options);
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


