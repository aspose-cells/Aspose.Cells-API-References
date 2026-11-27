---
title: "PivotFieldCollection.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFieldCollection metod. Lägger till ett PivotField‑objekt till den specifika typen PivotFields"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfieldcollection/add/
---
## PivotFieldCollection.Add method

Lägger till ett PivotField‑objekt till den specifika typen PivotFields.

```csharp
public int Add(PivotField pivotField)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivotField | PivotField | ett PivotField‑objekt. |

### Returvärde

indexet för PivotField‑objektet i dessa PivotFields.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldCollectionMethodAddWithPivotFieldDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook("sample_pivot_table.xlsx");
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till den första pivottabellen
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Uppdatera pivot‑tabellens data
            pivotTable.RefreshData();
            
            // Lägg till datafält i kolumnfältområdet med Add‑metoden
            pivotTable.ColumnFields.Add(pivotTable.DataField);
            
            // Beräkna pivottabellsdata
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("output_pivot_table.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


