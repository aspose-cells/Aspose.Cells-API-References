---
title: "TxtLoadOptions.Separator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtLoadOptions. Ottiene e imposta il separatore di caratteri del file di testo"
type: docs
url: /it/net/aspose.cells/txtloadoptions/separator/
---
## TxtLoadOptions.Separator property

Ottiene e imposta il separatore di caratteri del file di testo.

```csharp
public char Separator { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertySeparatorDemo
    {
        public static void Run()
        {
            // Crea dati di esempio e salva con separatore personalizzato
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.Separator = '*';
            workbook.Save("output.csv", saveOptions);

            // Carica il file salvato con lo stesso separatore
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.Separator = '*';
            Workbook loadedWorkbook = new Workbook("output.csv", loadOptions);

            // Verifica i dati caricati
            Worksheet loadedSheet = loadedWorkbook.Worksheets[0];
            Console.WriteLine("A1: " + loadedSheet.Cells["A1"].StringValue);
            Console.WriteLine("B1: " + loadedSheet.Cells["B1"].StringValue);
        }
    }
}
```

### Vedi anche

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


