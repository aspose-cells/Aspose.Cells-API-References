---
title: "TxtSaveOptions.Separator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtSaveOptions. Ottiene e imposta il delimitatore di carattere del file di testo"
type: docs
url: /it/net/aspose.cells/txtsaveoptions/separator/
---
## TxtSaveOptions.Separator property

Ottiene e imposta il delimitatore di caratteri del file di testo.

```csharp
public char Separator { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertySeparatorDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con dati di test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Configura le opzioni di salvataggio TXT con separatore virgola
            TxtSaveOptions txtSaveOptions = new TxtSaveOptions();
            txtSaveOptions.Separator = ',';
            txtSaveOptions.Encoding = System.Text.Encoding.UTF8;

            // Salva la cartella di lavoro come CSV con separatore virgola
            string outputPath = "output.csv";
            workbook.Save(outputPath, txtSaveOptions);

            // Visualizza il contenuto del file salvato
            Console.WriteLine("File saved with comma separator:");
            Console.WriteLine(File.ReadAllText(outputPath));
        }
    }
}
```

### Vedi anche

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


