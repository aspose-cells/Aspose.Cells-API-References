---
title: "PivotItem.PositionInSameParentNode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PivotItem. Specifica l'indice di posizione nei PivotItems sotto lo stesso nodo genitore"
type: docs
url: /it/net/aspose.cells.pivot/pivotitem/positioninsameparentnode/
---
## PivotItem.PositionInSameParentNode property

Specificare l'indice di posizione nei PivotItems sotto lo stesso nodo genitore.

```csharp
[Obsolete("Use PivotTable.MoveItem(PivotFieldType, string[],bool,int) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int PositionInSameParentNode { get; set; }
```

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo PivotTable.MoveItem(PivotFieldType, string[],bool,int). Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyPositionInSameParentNodeDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file Excel di origine
            Workbook workbook = new Workbook("PivotTest3.xlsx");
            
            // Aggiungi un nuovo foglio di lavoro per la tabella pivot
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            Worksheet dataSheet = workbook.Worksheets["New Hardware - Yearly"];

            // Aggiungi tabella pivot
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int index = pivotTables.Add("='New Hardware - Yearly'!A1:D621", "A3", "PivotTable");
            PivotTable pivotTable = pivotTables[index];

            // Aggiungi campi alla tabella pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Vendor");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "2014");

            // Configura la tabella pivot
            PivotField vendorField = pivotTable.RowFields["Vendor"];
            vendorField.SetSubtotals(PivotFieldSubtotalType.None, true);
            pivotTable.ShowColumnGrandTotals = false;

            // Aggiorna e calcola i dati
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Dimostra la proprietà PositionInSameParentNode
            PivotItemCollection items = pivotTable.RowFields["Item"].PivotItems;
            
            // Imposta le posizioni all'interno dello stesso nodo genitore
            items["4H12"].PositionInSameParentNode = 1;
            items["DIF400"].PositionInSameParentNode = 2;
            
            // Ricalcola dopo aver modificato le posizioni
            pivotTable.CalculateData();
            
            // Imposta le posizioni per un altro gruppo
            items["CA32"].PositionInSameParentNode = 1;
            items["AAA3"].PositionInSameParentNode = 2;

            // Salva la cartella di lavoro
            workbook.Save("PivotTableWithPositionInSameParentNode.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


