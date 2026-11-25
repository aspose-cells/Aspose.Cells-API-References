---
title: "FileFormatInfo.LoadFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FileFormatInfo. Ottiene il formato di caricamento rilevato"
type: docs
url: /it/net/aspose.cells/fileformatinfo/loadformat/
---
## FileFormatInfo.LoadFormat property

Ottiene il formato di caricamento rilevato.

```csharp
public LoadFormat LoadFormat { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatInfoPropertyLoadFormatDemo
    {
        public static void Run()
        {
            // Il percorso della directory dei documenti.
            string filePath = "data/";
            
            // Rileva il formato del file
            string fileName = "SAMPLE_XLS_ISSUE.XLS";
            var fileFormatInfo = FileFormatUtil.DetectFileFormat(filePath + fileName);
            Console.WriteLine("Detected LoadFormat: " + fileFormatInfo.LoadFormat);

            // Carica il file con il formato corretto
            LoadOptions loadOptions = new LoadOptions(LoadFormat.MHtml);
            var workbook = new Workbook(filePath + fileName, loadOptions);
            
            // Elabora la cartella di lavoro
            workbook.Worksheets[0].AutoFitColumns();
            workbook.Save(filePath + "output.xlsx");
        }
    }
}
```

### Vedi anche

* enum [LoadFormat](../../loadformat/)
* class [FileFormatInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


