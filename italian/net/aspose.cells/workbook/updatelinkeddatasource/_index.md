---
title: "Workbook.UpdateLinkedDataSource"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Workbook. Se questo workbook contiene collegamenti esterni a un'altra fonte di dati, Aspose.Cells cercherà di recuperare i dati più recenti dalle fonti fornite."
type: docs
url: /it/net/aspose.cells/workbook/updatelinkeddatasource/
---
## Workbook.UpdateLinkedDataSource method

Se questa cartella di lavoro contiene collegamenti esterni a un'altra fonte di dati, Aspose.Cells cercherà di recuperare i dati più recenti dalle fonti fornite.

```csharp
public void UpdateLinkedDataSource(Workbook[] externalWorkbooks)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| externalWorkbooks | Workbook[] | Workbook che verranno usati per aggiornare i dati dei collegamenti esterni a cui fa riferimento questo workbook. La corrispondenza di questi workbook con i collegamenti esterni è determinata da [`FileName`](../filename/) e [`DataSource`](../../externallink/datasource/). Pertanto, assicurati che [`FileName`](../filename/) sia stato specificato con il valore corretto per ogni workbook in modo che possano essere collegati al collegamento esterno corrispondente. |

### Osservazioni

Se non viene trovato il collegamento esterno corrispondente per un workbook, quel workbook verrà ignorato. Pertanto, quando imposti in seguito una formula con un nuovo collegamento esterno che desideri associare al workbook ignorato, il collegamento non potrà essere effettuato finché non richiami nuovamente questo metodo con quei workbook.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodUpdateLinkedDataSourceWithWorkbookDemo
    {
        public static void Run()
        {
            // Crea un workbook principale con riferimenti esterni
            Workbook mainWorkbook = new Workbook();
            Worksheet mainSheet = mainWorkbook.Worksheets[0];
            mainSheet.Cells["A1"].Formula = "=[ExternalWorkbook.xlsx]Sheet1!A1";

            // Crea un workbook esterno che verrà collegato
            Workbook externalWorkbook = new Workbook();
            Worksheet externalSheet = externalWorkbook.Worksheets[0];
            externalSheet.Cells["A1"].Value = "Updated External Value";

            try
            {
                // Chiama UpdateLinkedDataSource con l'array di workbook esterni
                mainWorkbook.UpdateLinkedDataSource(new Workbook[] { externalWorkbook });

                // Calcola le formule per aggiornare il riferimento
                mainWorkbook.CalculateFormula();

                // Visualizza il valore aggiornato
                Console.WriteLine("Updated value in main workbook: " + mainSheet.Cells["A1"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UpdateLinkedDataSource method: {ex.Message}");
            }

            // Salva il risultato
            mainWorkbook.Save("UpdateLinkedDataSourceDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


