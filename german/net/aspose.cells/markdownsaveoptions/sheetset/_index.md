---
title: "MarkdownSaveOptions.SheetSet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MarkdownSaveOptions‑Eigenschaft. Gibt die zu rendernden Blätter zurück oder legt sie fest. Standard ist alle sichtbaren Blätter in der Arbeitsmappe Active"
type: docs
url: /de/net/aspose.cells/markdownsaveoptions/sheetset/
---
## MarkdownSaveOptions.SheetSet property

Gibt die zu rendernden Blätter zurück oder legt sie fest. Standard ist alle sichtbaren Blätter in der Arbeitsmappe: [`Active`](../../../aspose.cells.rendering/sheetset/active/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Hinweise

Das Set wird ignoriert, wenn es in [`SheetRender`](../../../aspose.cells.rendering/sheetrender/) verwendet wird

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markdown;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Cells["A1"].PutValue("Sheet1 Data");
            
            // Füge ein zweites Arbeitsblatt hinzu
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["A1"].PutValue("Sheet2 Data");

            // Erstelle Markdown‑Speicheroptionen
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
            
            // Speichere alle Blätter als Markdown
            saveOptions.SheetSet = SheetSet.All;
            workbook.Save("output_all_sheets.md", saveOptions);
            
            // Nur das erste Blatt speichern
            saveOptions.SheetSet = new SheetSet(new int[] { 0 });
            workbook.Save("output_first_sheet.md", saveOptions);
        }
    }
}
```

### Siehe auch

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


