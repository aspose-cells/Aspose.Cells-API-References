---
title: "HtmlSaveOptions.ExportCellCoordinate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare le coordinate Excel delle celle non vuote durante il salvataggio del file in html. Il valore predefinito è false. Se desideri importare l'html di output in Excel, mantieni il valore predefinito."
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportcellcoordinate/
---
## HtmlSaveOptions.ExportCellCoordinate property

Indica se esportare le coordinate Excel delle celle non vuote quando si salva il file in html. Il valore predefinito è false. Se vuoi importare l'html di output in Excel, mantieni il valore predefinito.

```csharp
public bool ExportCellCoordinate { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportCellCoordinateDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // Crea le opzioni di salvataggio HTML e abilita ExportCellCoordinate
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportCellCoordinate = true;

            // Salva la cartella di lavoro come HTML con le coordinate delle celle
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML with cell coordinates exported successfully.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


