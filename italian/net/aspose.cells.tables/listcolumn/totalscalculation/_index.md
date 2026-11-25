---
title: "ListColumn.TotalsCalculation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListColumn. Ottiene e imposta il tipo di calcolo nella riga Totali della colonna dell'elenco"
type: docs
url: /it/net/aspose.cells.tables/listcolumn/totalscalculation/
---
## ListColumn.TotalsCalculation property

Ottiene e imposta il tipo di calcolo nella riga Totali della colonna dell'elenco.

```csharp
public TotalsCalculation TotalsCalculation { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyTotalsCalculationDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["A4"].PutValue("Item 3");
            worksheet.Cells["B4"].PutValue(200);

            // Crea un oggetto elenco
            int listObjIndex = worksheet.ListObjects.Add(0, 0, 4, 1, true);
            ListObject listObj = worksheet.ListObjects[listObjIndex];
            listObj.ShowTotals = true;
            
            // Imposta il calcolo dei totali per la seconda colonna
            listObj.ListColumns[1].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;

            // Salva la cartella di lavoro
            workbook.Save("ListColumnTotalsCalculationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [TotalsCalculation](../../totalscalculation/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


