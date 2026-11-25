---
title: "TxtSaveOptions.TrimLeadingBlankRowAndColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà TxtSaveOptions. Indica se le righe e le colonne vuote iniziali devono essere eliminate come fa ms excel. Il valore predefinito è true"
type: docs
url: /it/net/aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn/
---
## TxtSaveOptions.TrimLeadingBlankRowAndColumn property

Indica se le righe e le colonne vuote iniziali devono essere eliminate come fa MS Excel. Il valore predefinito è true.

```csharp
public bool TrimLeadingBlankRowAndColumn { get; set; }
```

### Osservazioni

Stessa regola di ms excel, una riga/colonna non verrà considerata vuota se ha uno stile personalizzato, anche se non contiene dati di cella. Quando si salva in modalità LightCells, questa opzione non ha effetto. L'utente dovrebbe controllare l'intervallo di output mediante l'implementazione di [`LightCellsDataProvider`](../lightcellsdataprovider/) o specificando [`ExportArea`](../exportarea/)

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyTrimLeadingBlankRowAndColumnDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio con alcuni dati e righe/colonne vuote
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati con righe e colonne vuote iniziali
            worksheet.Cells["C3"].PutValue("Data1");
            worksheet.Cells["D4"].PutValue("Data2");
            worksheet.Cells["E5"].PutValue("Data3");

            // Salva senza eliminare gli spazi vuoti iniziali
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.TrimLeadingBlankRowAndColumn = false;
            workbook.Save("output_with_blanks.csv", saveOptions);

            // Salva eliminando gli spazi vuoti iniziali
            saveOptions.TrimLeadingBlankRowAndColumn = true;
            workbook.Save("output_trimmed.csv", saveOptions);

            Console.WriteLine("Files saved successfully. Compare output_with_blanks.csv and output_trimmed.csv to see the difference.");
        }
    }
}
```

### Vedi anche

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


