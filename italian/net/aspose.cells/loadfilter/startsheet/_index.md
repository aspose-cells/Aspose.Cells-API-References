---
title: "LoadFilter.StartSheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo LoadFilter. Prepara le opzioni di filtro prima di caricare il foglio di lavoro specificato. L'implementazione dell'utente di LoadFilter può modificare qui le LoadDataFilterOptions per indicare come caricare i dati per questo foglio di lavoro"
type: docs
url: /it/net/aspose.cells/loadfilter/startsheet/
---
## LoadFilter.StartSheet method

Prepara le opzioni di filtro prima di caricare il foglio di lavoro specificato. L'implementazione dell'utente di LoadFilter può modificare le LoadDataFilterOptions qui per indicare come caricare i dati per questo foglio di lavoro.

```csharp
public virtual void StartSheet(Worksheet sheet)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| foglio | Worksheet | Il foglio di lavoro da caricare. Ci sono solo poche proprietà che possono essere usate per l'oggetto foglio di lavoro fornito qui perché la maggior parte dei dati e delle proprietà non sono stati caricati. Le proprietà disponibili sono: Name, Index, VisibilityType |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterMethodStartSheetWithWorksheetDemo
    {
        // Crea una classe di filtro di caricamento personalizzata che estende LoadFilter
        class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                Console.WriteLine($"Processing sheet: {sheet.Name}");
                // Puoi aggiungere logica personalizzata qui per gestire fogli specifici
            }
        }

        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "TestSheet";

            // Crea un'istanza del nostro filtro di caricamento personalizzato
            CustomLoadFilter loadFilter = new CustomLoadFilter();

            try
            {
                // Chiama il metodo StartSheet con il parametro worksheet
                loadFilter.StartSheet(worksheet);
                
                Console.WriteLine("StartSheet method executed successfully");
                
                // Aggiungi alcuni dati per dimostrare che il foglio è accessibile
                worksheet.Cells["A1"].PutValue("StartSheet Demo");
                worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartSheet method: {ex.Message}");
            }
            
            // Salva il risultato
            workbook.Save("LoadFilterStartSheetDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../../worksheet/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


