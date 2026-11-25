---
title: "TxtLoadOptions.SeparatorString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtLoadOptions. Ottiene e imposta un valore stringa come separatore"
type: docs
url: /it/net/aspose.cells/txtloadoptions/separatorstring/
---
## TxtLoadOptions.SeparatorString property

Ottiene e imposta un valore stringa come separatore.

```csharp
public string SeparatorString { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtLoadOptionsPropertySeparatorStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta dati di esempio con separatore personalizzato
            worksheet.Cells["A1"].PutValue("John&Doe");
            worksheet.Cells["B1"].PutValue("30");
            worksheet.Cells["A2"].PutValue("Jane&Smith");
            worksheet.Cells["B2"].PutValue("25");

            // Salva con separatore personalizzato
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.SeparatorString = "&";
            workbook.Save("output.csv", saveOptions);

            // Carica con lo stesso separatore
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.SeparatorString = "&";
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


