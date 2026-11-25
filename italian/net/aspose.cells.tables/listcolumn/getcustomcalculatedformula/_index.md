---
title: "ListColumn.GetCustomCalculatedFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "metodo ListColumn. Ottiene la formula di questa colonna di elenco"
type: docs
url: /it/net/aspose.cells.tables/listcolumn/getcustomcalculatedformula/
---
## ListColumn.GetCustomCalculatedFormula method

Ottiene la formula di questa colonna dell'elenco.

```csharp
public string GetCustomCalculatedFormula(bool isR1C1, bool isLocal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | Booleano | Indica se la formula deve essere formattata come R1C1. |
| isLocal | Booleano | Indica se la formula deve essere formattata in base alla lingua locale. |

### Valore di ritorno

La formula di questa colonna di elenco.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnMethodGetCustomCalculatedFormulaWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Crea dati di esempio
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Mary");
            sheet.Cells["B1"].PutValue("Score");
            sheet.Cells["B2"].PutValue(85);
            sheet.Cells["B3"].PutValue(92);
            
            // Crea un oggetto elenco
            int index = sheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = sheet.ListObjects[index];
            
            // Aggiungi una colonna calcolata
            ListColumn calcColumn = listObject.ListColumns[1];
            calcColumn.Formula = "=WEEKNUM([@Score])";
            
            // Ottieni la formula calcolata personalizzata
            string formula = listObject.ListColumns[1].GetCustomCalculatedFormula(false, false);
            
            // Restituisci il risultato
            Console.WriteLine("Calculated Formula: " + formula);
        }
    }
}
```

### Vedi anche

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


