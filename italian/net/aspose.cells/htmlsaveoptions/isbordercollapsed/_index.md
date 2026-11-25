---
title: "HtmlSaveOptions.IsBorderCollapsed"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se i bordi della tabella sono compressi. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/isbordercollapsed/
---
## HtmlSaveOptions.IsBorderCollapsed property

Indica se i bordi della tabella sono compressi. Il valore predefinito è true.

```csharp
public bool IsBorderCollapsed { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using System.Threading;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyIsBorderCollapsedDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio e bordi
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["B2"].PutValue("With Borders");
            worksheet.Cells["B2"].SetStyle(style);

            // Imposta la cultura per la dimostrazione
            var culture = new System.Globalization.CultureInfo("de-DE");
            Thread.CurrentThread.CurrentCulture = culture;
            Thread.CurrentThread.CurrentUICulture = culture;
            workbook.Settings.CultureInfo = culture;

            // Crea le opzioni di salvataggio HTML e imposta IsBorderCollapsed
            HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
            saveOptions.IsBorderCollapsed = false;

            // Salva la cartella di lavoro con le opzioni HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "HtmlWithBorders.html");
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("File saved with collapsed borders: " + outputPath);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


