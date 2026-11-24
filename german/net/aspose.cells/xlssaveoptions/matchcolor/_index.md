---
title: "XlsSaveOptions.MatchColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "XlsSaveOptions-Eigenschaft. Gibt an, ob die Schriftfarbe abgeglichen wird, da es 56 Farben in der Standardfarbpalette gibt"
type: docs
url: /de/net/aspose.cells/xlssaveoptions/matchcolor/
---
## XlsSaveOptions.MatchColor property

Gibt an, ob die Schriftfarbe angepasst wird, da es 56 Farben in der Standardfarbpalette gibt.

```csharp
public bool MatchColor { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyMatchColorDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe und greifen Sie auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf die Zelle B2 zu und setzen Sie einen Text mit einer bestimmten Schriftfarbe
            Cell cellB2 = worksheet.Cells["B2"];
            cellB2.PutValue("Sample Text");
            
            // Setzen Sie die Schriftfarbe auf Blau
            Style style = cellB2.GetStyle();
            style.Font.Color = Color.Blue;
            cellB2.SetStyle(style);

            // Erstellen Sie Speicheroptionen mit MatchColor auf true gesetzt
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            saveOptions.MatchColor = true;

            // Speichern Sie die Arbeitsmappe mit den Optionen
            workbook.Save("output.xls", saveOptions);

            // Laden Sie die gespeicherte Datei erneut, um zu überprüfen, ob die Farbe erhalten blieb
            Workbook savedWorkbook = new Workbook("output.xls");
            Cell savedCellB2 = savedWorkbook.Worksheets[0].Cells["B2"];
            
            // Überprüfen Sie, ob die Schriftfarbe weiterhin Blau ist
            Color savedColor = savedCellB2.GetStyle().Font.Color;
            Console.WriteLine("Saved font color: " + savedColor.ToString());
        }
    }
}
```

### Siehe auch

* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


