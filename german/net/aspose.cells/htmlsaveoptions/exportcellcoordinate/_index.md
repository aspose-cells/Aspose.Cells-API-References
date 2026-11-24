---
title: "HtmlSaveOptions.ExportCellCoordinate"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions property. Gibt an, ob beim Speichern der Datei als HTML die Excel-Koordinaten nicht leerer Zellen exportiert werden. Der Standardwert ist false. Wenn Sie das erzeugte HTML nach Excel importieren möchten, behalten Sie bitte den Standardwert bei."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/exportcellcoordinate/
---
## HtmlSaveOptions.ExportCellCoordinate property

Gibt an, ob excel-Koordinaten nicht leerer Zellen beim Speichern der Datei als html exportiert werden. Der Standardwert ist false. Wenn Sie das erzeugte html in excel importieren möchten, belassen Sie bitte den Standardwert.

```csharp
public bool ExportCellCoordinate { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportCellCoordinateDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // HTML-Speicheroptionen erstellen und ExportCellCoordinate aktivieren
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportCellCoordinate = true;

            // Arbeitsmappe als HTML mit Zellkoordinaten speichern
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML with cell coordinates exported successfully.");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


