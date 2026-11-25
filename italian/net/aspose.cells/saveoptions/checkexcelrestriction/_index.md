---
title: "SaveOptions.CheckExcelRestriction"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SaveOptions. Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando si inserisce un valore più lungo di 32K verrà troncato"
type: docs
url: /it/net/aspose.cells/saveoptions/checkexcelrestriction/
---
## SaveOptions.CheckExcelRestriction property

Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, verrà troncato.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Disabilita il controllo delle restrizioni di Excel
            workbook.Settings.CheckExcelRestriction = false;

            // Accedi al primo foglio di lavoro e alle celle
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Crea una stringa più lunga del limite normale di Excel
            string longString = new string('x', 32767) + " Testing Excel restriction";
            
            // Inserisci la stringa lunga nella cella A1
            cells["A1"].PutValue(longString);

            // Configura le opzioni di salvataggio per aggirare le restrizioni
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CheckExcelRestriction = false;

            // Salva la cartella di lavoro
            workbook.Save("output_without_restrictions.xlsx", saveOptions);

            // Carica il file salvato con le restrizioni disabilitate
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.CheckExcelRestriction = false;
            Workbook loadedWorkbook = new Workbook("output_without_restrictions.xlsx", loadOptions);

            // Verifica che la stringa lunga sia stata preservata
            string loadedValue = loadedWorkbook.Worksheets[0].Cells["A1"].StringValue;
            Console.WriteLine("Loaded string length: " + loadedValue.Length);
            Console.WriteLine("First 50 chars: " + loadedValue.Substring(0, 50));
            Console.WriteLine("Last 50 chars: " + loadedValue.Substring(loadedValue.Length - 50));
        }
    }
}
```

### Vedi anche

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


