---
title: "CopyOptions.ReferToSheetWithSameName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CopyOptions. In MS Excel, quando si copiano formule che fanno riferimento ad altri fogli durante la copia di un foglio di lavoro in un altro, le formule copiate dovrebbero fare riferimento alla cartella di lavoro di origine. Tuttavia, in alcune situazioni l'utente potrebbe aver bisogno che le formule copiate facciano riferimento a fogli con lo stesso nome nella stessa cartella di lavoro, ad esempio quando quei fogli sono stati copiati prima di questa operazione di copia; in tal caso questa proprietà deve rimanere impostata su true."
type: docs
url: /it/net/aspose.cells/copyoptions/refertosheetwithsamename/
---
## CopyOptions.ReferToSheetWithSameName property

In MS Excel, quando si copiano formule che fanno riferimento ad altri fogli di lavoro durante la copia di un foglio in un altro, le formule copiate dovrebbero fare riferimento alla cartella di lavoro di origine. Tuttavia, in alcune situazioni l'utente potrebbe aver bisogno che le formule copiate facciano riferimento a fogli con lo stesso nome nella stessa cartella di lavoro, ad esempio quando quei fogli sono stati copiati prima di questa operazione di copia; in tal caso questa proprietà dovrebbe rimanere impostata su true.

```csharp
public bool ReferToSheetWithSameName { get; set; }
```

### Osservazioni

Il valore predefinito è true.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyReferToSheetWithSameNameDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro modello con dati di esempio
            Workbook templateWorkbook = new Workbook();
            Worksheet templateSheet1 = templateWorkbook.Worksheets[0];
            templateSheet1.Name = "Data";
            templateSheet1.Cells["A1"].PutValue("Value");
            templateSheet1.Cells["A2"].PutValue(10);
            templateSheet1.Cells["A3"].PutValue(20);
            
            Worksheet templateSheet2 = templateWorkbook.Worksheets.Add("Summary");
            templateSheet2.Cells["B2"].Formula = "=SUM(Data!A2:A3)";

            // Crea la cartella di lavoro di output
            Workbook outputWorkbook = new Workbook();
            outputWorkbook.Worksheets.Clear();

            // Copia i fogli di lavoro con ReferToSheetWithSameName abilitato
            foreach (Worksheet sheet in templateWorkbook.Worksheets)
            {
                outputWorkbook.Worksheets.Add(sheet.Name);
                CopyOptions options = new CopyOptions();
                options.ReferToSheetWithSameName = true;
                outputWorkbook.Worksheets[sheet.Name].Copy(sheet, options);
            }

            // Verifica che la formula faccia riferimento al foglio corretto
            Console.WriteLine("Formula in output workbook: " + 
                outputWorkbook.Worksheets["Summary"].Cells["B2"].Formula);
        }
    }
}
```

### Vedi anche

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


