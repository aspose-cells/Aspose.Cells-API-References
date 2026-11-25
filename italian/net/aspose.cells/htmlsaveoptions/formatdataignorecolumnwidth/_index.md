---
title: "HtmlSaveOptions.FormatDataIgnoreColumnWidth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se mostrare tutti i dati formattati della cella quando supera la larghezza della colonna. Se true ignora la larghezza della colonna e tutti i dati della cella verranno esportati. Se false i dati verranno esportati come in Excel. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/formatdataignorecolumnwidth/
---
## HtmlSaveOptions.FormatDataIgnoreColumnWidth property

Indica se mostrare tutti i dati formattati della cella quando supera la larghezza della colonna. Se true, la larghezza della colonna viene ignorata e tutti i dati della cella verranno esportati. Se false, i dati verranno esportati come in Excel. Il valore predefinito è false.

```csharp
public bool FormatDataIgnoreColumnWidth { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyFormatDataIgnoreColumnWidthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta dati di esempio e larghezza della colonna
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B1"].PutValue("Longer Text That Might Be Truncated");
            worksheet.Cells.SetColumnWidth(0, 10); // Narrow column
            worksheet.Cells.SetColumnWidth(1, 5);  // Very narrow column

            // Crea opzioni di salvataggio HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Dimostra la proprietà FormatDataIgnoreColumnWidth
            saveOptions.FormatDataIgnoreColumnWidth = true; // Text won't be truncated by column width
            
            // Salva con impostazioni diverse per mostrare l'effetto
            workbook.Save("HtmlWithIgnoreColumnWidth.html", saveOptions);
            
            saveOptions.FormatDataIgnoreColumnWidth = false; // Text may be truncated by column width
            workbook.Save("HtmlWithoutIgnoreColumnWidth.html", saveOptions);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


