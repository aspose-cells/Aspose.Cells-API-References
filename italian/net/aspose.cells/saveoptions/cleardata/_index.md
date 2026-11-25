---
title: "SaveOptions.ClearData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SaveOptions. Rende la cartella di lavoro vuota dopo aver salvato il file"
type: docs
url: /it/net/aspose.cells/saveoptions/cleardata/
---
## SaveOptions.ClearData property

Rendi la cartella di lavoro vuota dopo aver salvato il file.

```csharp
public bool ClearData { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyClearDataDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di test
            worksheet.Cells["A1"].PutValue("Tabelle1");
            worksheet.Cells["B3"].PutValue(3);

            // Configura le opzioni di salvataggio con ClearData = false
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.ClearData = false;
            saveOptions.Separator = ',';

            // Salva la cartella di lavoro
            string outputPath = "output_with_cleardata_false.csv";
            workbook.Save(outputPath, saveOptions);

            // Ricarica per verificare che i dati siano stati conservati
            Workbook loadedWorkbook = new Workbook(outputPath);
            Cells cells = loadedWorkbook.Worksheets[0].Cells;
            
            Console.WriteLine("A1 value: " + cells["A1"].StringValue);
            Console.WriteLine("B3 value: " + cells["B3"].IntValue);
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


