---
title: "Worksheet.GetSelectedRanges"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Ottiene gli intervalli di celle selezionati nel foglio di calcolo del designer"
type: docs
url: /it/net/aspose.cells/worksheet/getselectedranges/
---
## Worksheet.GetSelectedRanges method

Ottiene gli intervalli selezionati di celle nel foglio di calcolo del designer.

```csharp
[Obsolete("Use Worksheet.GetSelectedAreas() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetSelectedRanges()
```

### Valore di ritorno

Un ArrayList che contiene gli intervalli selezionati.

### Osservazioni

NOTA: questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo Worksheet.GetSelectedAreas(). Questa proprietà sarà rimossa tra 12 mesi a partire da marzo 2025. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class WorksheetMethodGetSelectedRangesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B2"].Value = "Test Value";

            try
            {
                // Nota: GetSelectedRanges è contrassegnato come obsoleto nella riflessione
                // Questo dimostra la chiamata al metodo come richiesto
                ArrayList selectedRanges = worksheet.GetSelectedRanges();

                // Visualizza il numero di intervalli selezionati
                Console.WriteLine($"Number of selected ranges: {selectedRanges.Count}");

                // Visualizza ogni intervallo selezionato
                foreach (var range in selectedRanges)
                {
                    Console.WriteLine($"Selected range: {range}");
                }

                // Salva la cartella di lavoro
                workbook.Save("GetSelectedRangesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


