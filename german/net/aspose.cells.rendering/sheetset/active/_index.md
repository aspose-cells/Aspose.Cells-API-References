---
title: "SheetSet.Active"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SheetSet-Eigenschaft. Gibt ein Set mit dem aktiven Blatt der Arbeitsmappe zurück"
type: docs
url: /de/net/aspose.cells.rendering/sheetset/active/
---
## SheetSet.Active property

Erhält ein Set mit dem aktiven Blatt der Arbeitsmappe.

```csharp
public static SheetSet Active { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyActiveDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit zwei Arbeitsblättern
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // Setzen Sie das zweite Arbeitsblatt als aktiv
            workbook.Worksheets.ActiveSheetIndex = 1;

            // Daten zu beiden Arbeitsblättern hinzufügen
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Active Sheet Data");

            // PDF-Speicheroptionen erstellen
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Nur das aktive Blatt speichern
            pdfSaveOptions.SheetSet = SheetSet.Active;
            workbook.Save("ActiveSheetOnly.pdf", pdfSaveOptions);

            // Alle Blätter zum Vergleich speichern
            pdfSaveOptions.SheetSet = SheetSet.All;
            workbook.Save("AllSheets.pdf", pdfSaveOptions);
        }
    }
}
```

### Siehe auch

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


