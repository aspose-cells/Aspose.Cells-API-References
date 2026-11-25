---
title: "WorkbookSettings.CheckExcelRestriction"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Indica se verificare le restrizioni del file Excel quando l'utente modifica oggetti correlati alle celle. Per esempio, Excel non consente l'inserimento di una stringa più lunga di 32K. Quando inserisci un valore più lungo di 32K, ad esempio tramite Cell.PutValuestring, se questa proprietà è true otterrai un'Exception. Se la proprietà è false accetteremo la tua stringa di input come valore della cella, così in seguito potrai esportare la stringa completa per altri formati di file come CSV. Tuttavia, se hai impostato un valore di questo tipo che è non valido per il formato file Excel, non dovresti salvare la cartella di lavoro in formato Excel successivamente. Altrimenti potrebbero verificarsi errori inaspettati nel file Excel generato"
type: docs
url: /it/net/aspose.cells/workbooksettings/checkexcelrestriction/
---
## WorkbookSettings.CheckExcelRestriction property

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
    public class WorkbookSettingsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Disabilita il controllo delle restrizioni di Excel
            workbook.Settings.CheckExcelRestriction = false;
            
            // Inserisci una stringa che supera i limiti normali di Excel
            string longString = new string('a', 40000);
            workbook.Worksheets[0].Cells["A1"].PutValue(longString);
            
            // Salva e ricarica per verificare che la restrizione sia stata aggirata
            string tempFile = Guid.NewGuid().ToString() + ".txt";
            workbook.Save(tempFile, new TxtSaveOptions());
            
            Workbook loadedWorkbook = new Workbook(tempFile, new LoadOptions { CheckExcelRestriction = false });
            Console.WriteLine("String length: " + loadedWorkbook.Worksheets[0].Cells["A1"].StringValue.Length);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


