---
title: "HtmlSaveOptions.ShowAllSheets"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob beim Speichern als einzelne HTML‑Datei alle Arbeitsblätter angezeigt werden sollen"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/showallsheets/
---
## HtmlSaveOptions.ShowAllSheets property

Gibt an, ob beim Speichern als einzelne HTML‑Datei alle Arbeitsblätter angezeigt werden.

```csharp
public bool ShowAllSheets { get; set; }
```

### Hinweise

Funktioniert nur, wenn [`SaveAsSingleFile`](../saveassinglefile/) True ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyShowAllSheetsDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit mehreren Arbeitsblättern
            Workbook workbook = new Workbook();
            
            // Füge Daten zum ersten Arbeitsblatt hinzu
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "FirstSheet";
            sheet1.Cells["A1"].PutValue("Sheet 1 Content");

            // Füge zweites Arbeitsblatt hinzu
            Worksheet sheet2 = workbook.Worksheets.Add("SecondSheet");
            sheet2.Cells["B2"].PutValue("Sheet 2 Content");

            // Füge drittes Arbeitsblatt hinzu
            Worksheet sheet3 = workbook.Worksheets.Add("ThirdSheet");
            sheet3.Cells["C3"].PutValue("Sheet 3 Content");

            // HTML‑Speicheroptionen erstellen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Setze die ShowAllSheets‑Eigenschaft auf true, um alle Arbeitsblätter zu exportieren
            saveOptions.ShowAllSheets = true;

            // Speichere die Arbeitsmappe mit allen sichtbaren Arbeitsblättern in HTML
            workbook.Save("ShowAllSheetsDemo.html", saveOptions);

            Console.WriteLine("HTML file with all sheets exported successfully.");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


