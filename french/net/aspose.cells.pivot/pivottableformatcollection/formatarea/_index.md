---
title: "PivotTableFormatCollection.FormatArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotTableFormatCollection. Formate la zone sélectionnée"
type: docs
url: /fr/net/aspose.cells.pivot/pivottableformatcollection/formatarea/
---
## PivotTableFormatCollection.FormatArea method

Formate la zone sélectionnée.

```csharp
public PivotTableFormat FormatArea(PivotFieldType axisType, int fieldPosition, 
    PivotFieldSubtotalType subtotalType, PivotTableSelectionType selectionType, bool isGrandRow, 
    bool isGrandColumn, Style style)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| axisType | PivotFieldType | La région du tableau croisé dynamique à laquelle cette règle s'applique. |
| fieldPosition | Int32 | Position du champ dans l'axe auquel cette règle s'applique. |
| subtotalType | PivotFieldSubtotalType | Le type de filtre de sous-total du champ pivot |
| selectionType | PivotTableSelectionType | Indique comment sélectionner les données. |
| isGrandRow | Boolean | Indique si les lignes de total général sont sélectionnées. |
| isGrandColumn | Boolean | Indique si les colonnes de total général sont sélectionnées. |
| style | Style | Le style qui s'applique à la zone du tableau croisé dynamique. |

### Exemples

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
            // Créer un classeur à partir du fichier source
            Workbook workbook = new Workbook("example.xlsx");
            
            // Accéder au tableau croisé dynamique
            PivotTable pt = workbook.Worksheets["PIVOT_VBA_SUBTOTALS"].PivotTables[0];
            
            // Créer un style pour le formatage
            Style style = workbook.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Red);
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.LightGray;
            style.BackgroundColor = Color.LightGray;

            // Formater la zone du tableau croisé dynamique
            pt.PivotFormats.FormatArea(
                PivotFieldType.Row, 
                0, 
                PivotFieldSubtotalType.Automatic, 
                PivotTableSelectionType.DataAndLabel, 
                false, 
                false, 
                style);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PivotTableFormat](../../pivottableformat/)
* enum [PivotFieldType](../../pivotfieldtype/)
* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* enum [PivotTableSelectionType](../../pivottableselectiontype/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


