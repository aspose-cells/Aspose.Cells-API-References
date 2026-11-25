---
title: "HtmlSaveOptions.HtmlSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore HtmlSaveOptions. Crea le opzioni per salvare un file html"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/htmlsaveoptions/
---
## HtmlSaveOptions() {#constructor}

Crea le opzioni per salvare il file html.

```csharp
public HtmlSaveOptions()
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Inizializza HtmlSaveOptions usando il costruttore
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportActiveWorksheetOnly = true;
            
            // Salva come HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "output.html");
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file saved to: " + outputPath);
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## HtmlSaveOptions(SaveFormat) {#constructor_1}

Crea le opzioni per salvare il file htm.

```csharp
public HtmlSaveOptions(SaveFormat saveFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveFormat | SaveFormat | Il formato del file. Deve essere uno dei seguenti tipi: Html o MHtml, altrimenti il formato salvato verrà impostato automaticamente su Html. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["C3"].PutValue(DateTime.Now);
            
            try
            {
                // Crea HtmlSaveOptions con il parametro SaveFormat
                HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
                
                // Imposta alcune proprietà
                saveOptions.PageTitle = "Aspose.Cells HTML Export";
                saveOptions.ExportActiveWorksheetOnly = true;
                saveOptions.ExportGridLines = true;
                
                // Salva la cartella di lavoro con HtmlSaveOptions
                workbook.Save("HtmlExportWithOptions.html", saveOptions);
                
                Console.WriteLine("HTML file saved successfully with HtmlSaveOptions(SaveFormat)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing HtmlSaveOptions constructor: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../saveformat/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


