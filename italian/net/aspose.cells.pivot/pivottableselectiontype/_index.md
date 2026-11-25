---
title: "Enum PivotTableSelectionType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Pivot.PivotTableSelectionType. Specifica cosa può essere selezionato in una PivotTable durante una selezione strutturata. Queste costanti possono essere combinate per selezionare più tipi."
type: docs
url: /it/net/aspose.cells.pivot/pivottableselectiontype/
---
## PivotTableSelectionType enumeration

Specifica cosa può essere selezionato in una PivotTable durante una selezione strutturata. Queste costanti possono essere combinate per selezionare più tipi.

```csharp
public enum PivotTableSelectionType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| DataAndLabel | `0` | Dati e etichette |
| DataOnly | `2` | Seleziona solo i dati |
| LabelOnly | `1` | Seleziona solo le etichette |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableSelectionTypeDemo
    {
        public static void PivotTableSelectionTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per la PivotTable
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(250);

            // Crea una PivotTable
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Aggiungi campi alla PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crea un PivotArea e imposta le sue proprietà
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.OnlyData = false;
            pivotArea.OnlyLabel = true;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.IsOutline = false;

            // Seleziona l'area con un tipo di selezione specifico
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            // Salva la cartella di lavoro
            workbook.Save("PivotTableSelectionTypeExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


