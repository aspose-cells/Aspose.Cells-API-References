---
title: "PaginatedSaveOptions.SheetSet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaginatedSaveOptions-Eigenschaft. Gibt die zu rendernden Tabellenblätter zurück oder legt sie fest. Standard ist, dass alle sichtbaren Tabellenblätter in der Arbeitsmappe sichtbar sind."
type: docs
url: /de/net/aspose.cells/paginatedsaveoptions/sheetset/
---
## PaginatedSaveOptions.SheetSet property

Ruft die zu rendernden Arbeitsblätter ab oder legt sie fest. Standard ist alle sichtbaren Arbeitsblätter in der Arbeitsmappe: [`Visible`](../../../aspose.cells.rendering/sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe mit zwei Arbeitsblättern
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Beispieldaten in beiden Tabellenblättern festlegen
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");

            // PDF-Speicheroptionen erstellen
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Nur das zweite Tabellenblatt mit SheetSet speichern
            pdfSaveOptions.SheetSet = new SheetSet(new int[] { 1 }); // 0-based index
            
            // Arbeitsmappe mit den angegebenen Tabellenblättern speichern
            workbook.Save("output.pdf", pdfSaveOptions);
        }
    }
}
```

### Siehe auch

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


