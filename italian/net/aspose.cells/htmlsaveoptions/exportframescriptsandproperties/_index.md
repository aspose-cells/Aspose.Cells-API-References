---
title: "HtmlSaveOptions.ExportFrameScriptsAndProperties"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se esportare script dei frame e proprietà del documento. Il valore predefinito è true. Se desideri importare il file html o mht in Excel, mantieni il valore predefinito"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportframescriptsandproperties/
---
## HtmlSaveOptions.ExportFrameScriptsAndProperties property

Indica se esportare gli script del frame e le proprietà del documento. Il valore predefinito è true. Se vuoi importare il file html o mht in Excel, mantieni il valore predefinito.

```csharp
public bool ExportFrameScriptsAndProperties { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportFrameScriptsAndPropertiesDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Imposta le opzioni di salvataggio HTML con ExportFrameScriptsAndProperties
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportFrameScriptsAndProperties = true;

            // Salva come HTML
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with ExportFrameScriptsAndProperties enabled.");
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


