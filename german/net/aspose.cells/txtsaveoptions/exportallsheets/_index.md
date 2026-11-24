---
title: "TxtSaveOptions.ExportAllSheets"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtSaveOptions-Eigenschaft. Gibt an, ob alle Arbeitsblätter in die Textdatei exportiert werden. Wenn sie false ist, wird nur das aktive Arbeitsblatt exportiert, genau wie bei MS Excel"
type: docs
url: /de/net/aspose.cells/txtsaveoptions/exportallsheets/
---
## TxtSaveOptions.ExportAllSheets property

Gibt an, ob alle Arbeitsblätter in die Textdatei exportiert werden. Wenn false, wird nur das aktive Arbeitsblatt exportiert, ähnlich wie in MS Excel.

```csharp
public bool ExportAllSheets { get; set; }
```

### Hinweise

Der Standardwert ist false.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportAllSheetsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit zwei Arbeitsblättern
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Füge beiden Arbeitsblättern Beispieldaten hinzu
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[0].Cells["A2"].PutValue(1);
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");
            workbook.Worksheets[1].Cells["A2"].PutValue(2);

            // Speichern mit ExportAllSheets=false (Standard)
            TxtSaveOptions saveOptions = new TxtSaveOptions(SaveFormat.Csv);
            workbook.Save("output_single_sheet.csv", saveOptions);

            // Speichern mit ExportAllSheets=true
            saveOptions.ExportAllSheets = true;
            workbook.Save("output_all_sheets.csv", saveOptions);
        }
    }
}
```

### Siehe auch

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


