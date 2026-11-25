---
title: "PivotAreaFilter.IsSubtotalSet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotAreaFilter. Restituisce quale subtotale è impostato per questo filtro"
type: docs
url: /it/net/aspose.cells.pivot/pivotareafilter/issubtotalset/
---
## PivotAreaFilter.IsSubtotalSet method

Ottiene quale subtotale è impostato per questo filtro.

```csharp
public bool IsSubtotalSet(PivotFieldSubtotalType subtotalType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | Il tipo di funzione subtotale. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaFilterMethodIsSubtotalSetWithPivotFieldSubtotalTypeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Aggiungi un campo di riga e configura i subtotali
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields["Category"];
            rowField.IsAutoSubtotals = true;
            rowField.SetSubtotals(PivotFieldSubtotalType.Automatic, true);

            // Crea un'area pivot e verifica l'impostazione del subtotale
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Row, "Category");
            
            // Dimostra l'uso di IsSubtotalSet
            bool isSubtotalSet = pivotArea.Filters[0].IsSubtotalSet(PivotFieldSubtotalType.Automatic);
            Console.WriteLine($"Is Automatic subtotal set: {isSubtotalSet}");

            // Salva la cartella di lavoro
            workbook.Save("PivotSubtotalDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


