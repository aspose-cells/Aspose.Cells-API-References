---
title: "HtmlSaveOptions.ExportWorksheetProperties"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare le proprietà del foglio di lavoro. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito."
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportworksheetproperties/
---
## HtmlSaveOptions.ExportWorksheetProperties property

Indica se esportare le proprietà del foglio di lavoro. Il valore predefinito è true. Se vuoi importare il file html o mht in Excel, mantieni il valore predefinito.

```csharp
public bool ExportWorksheetProperties { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorksheetPropertiesDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con dati di test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");

            // Imposta le opzioni di salvataggio HTML con ExportWorksheetProperties disabilitato
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportWorksheetProperties = false;
            
            // Salva con le proprietà del foglio di lavoro disabilitate
            workbook.Save("output_without_worksheet_props.html", options);

            // Abilita l'esportazione delle proprietà del foglio di lavoro
            options.ExportWorksheetProperties = true;
            
            // Salva con le proprietà del foglio di lavoro abilitate
            workbook.Save("output_with_worksheet_props.html", options);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


