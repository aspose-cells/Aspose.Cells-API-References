---
title: "ListColumn.SetCustomTotalsRowFormula"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "metodo ListColumn. Ottiene la formula della riga totale di questa colonna di elenco"
type: docs
url: /it/net/aspose.cells.tables/listcolumn/setcustomtotalsrowformula/
---
## ListColumn.SetCustomTotalsRowFormula method

Ottiene la formula della riga dei totali di questa colonna dell'elenco.

```csharp
public void SetCustomTotalsRowFormula(string formula, bool isR1C1, bool isLocal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | String | la formula per questa colonna di elenco. |
| isR1C1 | Booleano | Indica se la formula deve essere formattata come R1C1. |
| isLocal | Booleano | Indica se la formula deve essere formattata in base alla lingua locale. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnMethodSetCustomTotalsRowFormulaWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);

            // Crea un oggetto elenco
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Abilita la riga totale e imposta una formula personalizzata
            listObject.ShowTotals = true;
            listObject.ListColumns[0].TotalsCalculation = TotalsCalculation.Custom;
            listObject.ListColumns[0].SetCustomTotalsRowFormula("=SUM([Column1])", false, false);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


