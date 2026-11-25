---
title: "HtmlSaveOptions.SaveAsSingleFile"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Indica se salvare l'HTML come file singolo. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/saveassinglefile/
---
## HtmlSaveOptions.SaveAsSingleFile property

Indica se salvare l'HTML come file unico. Il valore predefinito è false.

```csharp
public bool SaveAsSingleFile { get; set; }
```

### Osservazioni

Se nel workbook ci sono più fogli di lavoro o altre risorse necessarie, come immagini, solitamente quei fogli e le altre risorse devono essere salvati in file separati. In alcuni scenari, l'utente potrebbe aver bisogno di ottenere un unico file risultante per comodità di trasferimento. In tal caso, l'utente può impostare questa proprietà su true.

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertySaveAsSingleFileDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Inizializza le opzioni di salvataggio HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.SaveAsSingleFile = true;
            saveOptions.ExportPageHeaders = true;
            
            // Salva il workbook come file HTML singolo
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            // Verifica che il file di output esista
            if (File.Exists(outputPath))
            {
                Console.WriteLine("HTML saved as single file successfully.");
            }
        }
    }
}
```

### Vedi anche

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


