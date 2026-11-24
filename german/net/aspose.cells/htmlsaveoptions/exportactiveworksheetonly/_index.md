---
title: "HtmlSaveOptions.ExportActiveWorksheetOnly"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob nur das aktive Arbeitsblatt in eine HTML‑Datei exportiert wird. Wenn true, wird nur das aktive Arbeitsblatt in die HTML‑Datei exportiert. Wenn false, wird die gesamte Arbeitsmappe in die HTML‑Datei exportiert. Der Standardwert ist false."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/exportactiveworksheetonly/
---
## HtmlSaveOptions.ExportActiveWorksheetOnly property

Gibt an, ob nur das aktive Arbeitsblatt in eine html-Datei exportiert wird. Wenn true, wird nur das aktive Arbeitsblatt in die html-Datei exportiert; wenn false, wird die gesamte Arbeitsmappe in die html-Datei exportiert. Der Standardwert ist false.

```csharp
public bool ExportActiveWorksheetOnly { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportActiveWorksheetOnlyDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit zwei Arbeitsblättern
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Füge beiden Arbeitsblättern Beispieldaten hinzu
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // Setze die HTML‑Speicheroptionen, um nur das aktive Arbeitsblatt zu exportieren
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = true;
            
            // Setze das erste Arbeitsblatt als aktiv
            workbook.Worksheets.ActiveSheetIndex = 0;
            
            // Speichere nur mit dem aktiven Arbeitsblatt
            workbook.Save("output_active_sheet_only.html", saveOptions);
            
            // Wechsle das aktive Arbeitsblatt und speichere erneut
            workbook.Worksheets.ActiveSheetIndex = 1;
            workbook.Save("output_active_sheet_only2.html", saveOptions);
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


