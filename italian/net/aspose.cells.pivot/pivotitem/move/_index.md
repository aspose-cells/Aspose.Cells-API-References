---
title: "PivotItem.Move"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotItem. Sposta l'elemento su o giù"
type: docs
url: /it/net/aspose.cells.pivot/pivotitem/move/
---
## Move(int, bool) {#move_1}

Sposta l'elemento su o giù

```csharp
[Obsolete("Use PivotTable.MoveItem(PivotFieldType, string[],bool,int) method  or PivotItem.Move(int) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Move(int offset, bool isSameParent)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| spostamento | Int32 | Il numero di spostamenti su o giù. Sposta l'elemento verso l'alto se questo è minore di zero; sposta l'elemento verso il basso se è maggiore di zero. |
| isSameParent | Booleano | Specificando se l'operazione di spostamento avviene nello stesso nodo genitore o meno |

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare PivotTable.MoveItem(PivotFieldType, string[],bool,int) o il metodo PivotItem.Move(int) invece. Questo metodo sarà rimosso 12 mesi dopo, a partire da novembre 2026. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemMethodMoveWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro con dati di esempio
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Crea dati di esempio per la tabella pivot
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(100);
            sheet.Cells["B3"].PutValue(200);
            sheet.Cells["B4"].PutValue(300);

            // Aggiungi tabella pivot
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Aggiungi campo riga
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Ottieni gli elementi pivot e dimostra il metodo Move
            PivotItemCollection items = pivotTable.RowFields[0].PivotItems;
            
            // Sposta il primo elemento alla posizione 1 (seconda posizione) con gli elementi figli
            items[0].Move(1, true);
            
            // Salva la cartella di lavoro
            wb.Save("PivotItemMoveDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Move(int) {#move}

Sposta l'elemento su o giù nel campo pivot

```csharp
public void Move(int offset)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| spostamento | Int32 | Il numero di spostamenti su o giù. Sposta l'elemento verso l'alto se questo è minore di zero; sposta l'elemento verso il basso se è maggiore di zero. |

### Vedi anche

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


