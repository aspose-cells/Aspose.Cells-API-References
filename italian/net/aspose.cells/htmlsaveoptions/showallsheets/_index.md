---
title: "HtmlSaveOptions.ShowAllSheets"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se mostrare tutti i fogli durante il salvataggio in un unico file HTML"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/showallsheets/
---
## HtmlSaveOptions.ShowAllSheets property

Indica se mostrare tutti i fogli quando si salva come file HTML unico.

```csharp
public bool ShowAllSheets { get; set; }
```

### Osservazioni

Funziona solo quando [`SaveAsSingleFile`](../saveassinglefile/) è True.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyShowAllSheetsDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro con più fogli
            Workbook workbook = new Workbook();
            
            // Aggiungi dati al primo foglio
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "FirstSheet";
            sheet1.Cells["A1"].PutValue("Sheet 1 Content");

            // Aggiungi il secondo foglio
            Worksheet sheet2 = workbook.Worksheets.Add("SecondSheet");
            sheet2.Cells["B2"].PutValue("Sheet 2 Content");

            // Aggiungi il terzo foglio
            Worksheet sheet3 = workbook.Worksheets.Add("ThirdSheet");
            sheet3.Cells["C3"].PutValue("Sheet 3 Content");

            // Crea opzioni di salvataggio HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Imposta la proprietà ShowAllSheets su true per esportare tutti i fogli
            saveOptions.ShowAllSheets = true;

            // Salva la cartella di lavoro con tutti i fogli visibili in HTML
            workbook.Save("ShowAllSheetsDemo.html", saveOptions);

            Console.WriteLine("HTML file with all sheets exported successfully.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


