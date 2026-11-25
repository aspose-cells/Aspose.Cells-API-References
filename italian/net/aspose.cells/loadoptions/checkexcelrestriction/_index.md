---
title: "LoadOptions.CheckExcelRestriction"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Ad esempio Excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, ad esempio tramite Cell.PutValuestring, se questa proprietà è true otterrai un'Exception. Se la proprietà è false accetteremo la tua stringa di input come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo che è non valido per il formato file Excel, non dovresti salvare la cartella di lavoro come formato file Excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file Excel generato."
type: docs
url: /it/net/aspose.cells/loadoptions/checkexcelrestriction/
---
## LoadOptions.CheckExcelRestriction property

Indica se verificare le restrizioni del file excel quando l'utente modifica oggetti correlati alle celle. Per esempio, excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, ad esempio tramite Cell.PutValue(string), se questa proprietà è true otterrai un'Exception. Se la proprietà è false, accetteremo la stringa inserita come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo non valido per il formato file excel, non dovresti salvare la workbook in formato excel in seguito. Altrimenti potrebbero verificarsi errori imprevisti nel file excel generato.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Disabilita il controllo delle restrizioni di Excel
            workbook.Settings.CheckExcelRestriction = false;

            // Accedi al primo foglio di lavoro e alle celle
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Crea una stringa più lunga del limite normale di Excel (32767 caratteri)
            string longString = new string('x', 32767) + " Testing Excel restriction";
            
            // Inserisci la stringa lunga nella cella A1
            cells["A1"].PutValue(longString);
            
            // Salva con il controllo delle restrizioni disabilitato
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CheckExcelRestriction = false;
            workbook.Save("output.xlsx", saveOptions);
            
            // Carica con il controllo delle restrizioni disabilitato
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.CheckExcelRestriction = false;
            Workbook loadedWorkbook = new Workbook("output.xlsx", loadOptions);
            
            // Verifica che la stringa lunga sia stata preservata
            string loadedValue = loadedWorkbook.Worksheets[0].Cells["A1"].StringValue;
            Console.WriteLine("String length: " + loadedValue.Length);
            Console.WriteLine("String matches: " + loadedValue.Equals(longString));
        }
    }
}
```

### Vedi anche

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


