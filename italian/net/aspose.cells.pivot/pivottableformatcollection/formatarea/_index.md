---
title: "PivotTableFormatCollection.FormatArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotTableFormatCollection metodo. Formatta l'area selezionata"
type: docs
url: /it/net/aspose.cells.pivot/pivottableformatcollection/formatarea/
---
## PivotTableFormatCollection.FormatArea method

Formatta l'area selezionata.

```csharp
public PivotTableFormat FormatArea(PivotFieldType axisType, int fieldPosition, 
    PivotFieldSubtotalType subtotalType, PivotTableSelectionType selectionType, bool isGrandRow, 
    bool isGrandColumn, Style style)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| axisType | PivotFieldType | La regione della PivotTable a cui si applica questa regola. |
| fieldPosition | Int32 | Posizione del campo all'interno dell'asse a cui si applica questa regola. |
| subtotalType | PivotFieldSubtotalType | Il tipo di filtro subtotale del campo pivot |
| selectionType | PivotTableSelectionType | Indica come selezionare i dati. |
| isGrandRow | Booleano | Indica se si stanno selezionando le righe del totale generale. |
| isGrandColumn | Booleano | Indica se si stanno selezionando le colonne del totale generale. |
| stile | Stile | Lo stile che si applica all'area della tabella pivot. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class PivotTableFormatCollectionMethodFormatAreaWithPivotFieldTypeInt32PivotFieldSDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro dal file sorgente
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accedi alla tabella pivot
            PivotTable pt = workbook.Worksheets["PIVOT_VBA_SUBTOTALS"].PivotTables[0];
            
            // Crea uno stile per la formattazione
            Style style = workbook.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Red);
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.LightGray;
            style.BackgroundColor = Color.LightGray;

            // Formatta l'area della tabella pivot
            pt.PivotFormats.FormatArea(
                PivotFieldType.Row, 
                0, 
                PivotFieldSubtotalType.Automatic, 
                PivotTableSelectionType.DataAndLabel, 
                false, 
                false, 
                style);

            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotTableFormat](../../pivottableformat/)
* enum [PivotFieldType](../../pivotfieldtype/)
* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* enum [PivotTableSelectionType](../../pivottableselectiontype/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


