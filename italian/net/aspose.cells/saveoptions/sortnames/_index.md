---
title: "SaveOptions.SortNames"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SaveOptions. Indica se ordinare i nomi definiti prima di salvare il file"
type: docs
url: /it/net/aspose.cells/saveoptions/sortnames/
---
## SaveOptions.SortNames property

Indica se ordinare i nomi definiti prima di salvare il file.

```csharp
public bool SortNames { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertySortNamesDemo
    {
        public static void Run()
        {
            // Crea un nuovo oggetto Workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Crea un intervallo denominato
            worksheet.Cells.CreateRange("A2:B3").Name = "MyDataRange";

            // Crea opzioni di salvataggio con SortNames abilitato
            XlsSaveOptions saveOptions = new XlsSaveOptions
            {
                SortNames = true
            };

            // Salva la cartella di lavoro
            workbook.Save("SortedNamesExample.xls", saveOptions);

            Console.WriteLine("Workbook saved with sorted named ranges.");
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


