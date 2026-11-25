---
title: "MarkdownSaveOptions.SheetSet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà MarkdownSaveOptions. Ottiene o imposta i fogli da renderizzare. Il valore predefinito è tutti i fogli visibili nella cartella di lavoro Active"
type: docs
url: /it/net/aspose.cells/markdownsaveoptions/sheetset/
---
## MarkdownSaveOptions.SheetSet property

Ottiene o imposta i fogli da renderizzare. Il valore predefinito è tutti i fogli visibili nella cartella di lavoro: [`Active`](../../../aspose.cells.rendering/sheetset/active/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Osservazioni

Il set viene ignorato quando viene utilizzato in [`SheetRender`](../../../aspose.cells.rendering/sheetrender/)

### Esempi

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
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Cells["A1"].PutValue("Sheet1 Data");
            
            // Aggiungi un secondo foglio di lavoro
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.Cells["A1"].PutValue("Sheet2 Data");

            // Crea le opzioni di salvataggio Markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
            
            // Salva tutti i fogli in markdown
            saveOptions.SheetSet = SheetSet.All;
            workbook.Save("output_all_sheets.md", saveOptions);
            
            // Salva solo il primo foglio
            saveOptions.SheetSet = new SheetSet(new int[] { 0 });
            workbook.Save("output_first_sheet.md", saveOptions);
        }
    }
}
```

### Vedi anche

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


