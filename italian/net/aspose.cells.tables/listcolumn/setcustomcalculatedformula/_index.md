---
title: "ListColumn.SetCustomCalculatedFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ListColumn. Imposta la formula per questa colonna dell'elenco"
type: docs
url: /it/net/aspose.cells.tables/listcolumn/setcustomcalculatedformula/
---
## ListColumn.SetCustomCalculatedFormula method

Imposta la formula per questa colonna dell'elenco.

```csharp
public void SetCustomCalculatedFormula(string formula, bool isR1C1, bool isLocal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | String | la formula per questa colonna di elenco. |
| isR1C1 | Booleano | Indica se la formula deve essere formattata come R1C1. |
| isLocal | Booleano | Indica se la formula deve essere formattata in base alla lingua locale. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnMethodSetCustomCalculatedFormulaWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea dati di esempio per la tabella
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B1"].PutValue("Total");

            // Crea tabella
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true); // Adjusted parameters to match correct overload
            ListObject table = worksheet.ListObjects[tableIndex];

            // Ottieni la seconda colonna dell'elenco
            ListColumn totalColumn = table.ListColumns[1];

            try
            {
                // Imposta una formula personalizzata usando la notazione A1 con locale standard
                totalColumn.SetCustomCalculatedFormula("=A2*1.1", false, false);
                
                Console.WriteLine("Custom formula set successfully.");
                Console.WriteLine($"Cell B2 formula: {worksheet.Cells["B2"].Formula}");
                Console.WriteLine($"Cell B3 formula: {worksheet.Cells["B3"].Formula}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("SetCustomCalculatedFormulaExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


