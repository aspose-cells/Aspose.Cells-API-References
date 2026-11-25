---
title: "HtmlSaveOptions.ExportSimilarBorderStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare lo stile di bordo simile quando lo stile di bordo non è supportato dai browser. Se desideri importare il file HTML o MHT in Excel, mantieni il valore predefinito. Il valore predefinito è false."
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportsimilarborderstyle/
---
## HtmlSaveOptions.ExportSimilarBorderStyle property

Indica se esportare lo stile di bordo simile quando lo stile di bordo non è supportato dai browser. Se vuoi importare il file html o mht in Excel, mantieni il valore predefinito. Il valore predefinito è false.

```csharp
public bool ExportSimilarBorderStyle { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportSimilarBorderStyleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con bordi.
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].SetStyle(CreateBorderStyle(workbook, CellBorderType.Medium));
            worksheet.Cells["B1"].PutValue("Similar Border");
            worksheet.Cells["B1"].SetStyle(CreateBorderStyle(workbook, CellBorderType.Medium));
            worksheet.Cells["C1"].PutValue("Different Border");
            worksheet.Cells["C1"].SetStyle(CreateBorderStyle(workbook, CellBorderType.Thin));

            // Crea opzioni di salvataggio HTML
            HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions(SaveFormat.Html)
            {
                ExportSimilarBorderStyle = true // Demonstrate the property
            };

            // Salva la cartella di lavoro
            workbook.Save("output.html", htmlSaveOptions);
        }

        private static Style CreateBorderStyle(Workbook workbook, CellBorderType borderType)
        {
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = borderType;
            style.Borders[BorderType.BottomBorder].LineStyle = borderType;
            style.Borders[BorderType.LeftBorder].LineStyle = borderType;
            style.Borders[BorderType.RightBorder].LineStyle = borderType;
            return style;
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


