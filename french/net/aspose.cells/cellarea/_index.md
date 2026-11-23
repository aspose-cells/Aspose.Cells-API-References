---
title: "Structure CellArea"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.CellArea struct. Représente une zone de cellules"
type: docs
url: /fr/net/aspose.cells/cellarea/
---
## CellArea structure

Représente une zone de cellules.

```csharp
public struct CellArea : IComparable
```

## Méthodes

| Nom | Description |
| --- | --- |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea_1)(string, string) | Crée une zone de cellules. |
| static [CreateCellArea](../../aspose.cells/cellarea/createcellarea/#createcellarea)(int, int, int, int) | Crée une zone de cellules. |
| [CompareTo](../../aspose.cells/cellarea/compareto/)(object) | Comparer deux objets CellArea selon leur coin supérieur gauche. |
| override [ToString](../../aspose.cells/cellarea/tostring/)() | Renvoie une chaîne qui représente l'objet de zone de cellules actuel. |

## Champs

| Nom | Description |
| --- | --- |
| [EndColumn](../../aspose.cells/cellarea/endcolumn/) | Obtient ou définit la colonne de fin de cette zone. |
| [EndRow](../../aspose.cells/cellarea/endrow/) | Obtient ou définit la ligne de fin de cette zone. |
| [StartColumn](../../aspose.cells/cellarea/startcolumn/) | Obtient ou définit la colonne de départ de cette zone. |
| [StartRow](../../aspose.cells/cellarea/startrow/) | Obtient ou définit la ligne de départ de cette zone. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellAreaDemo
    {
        public static void CellAreaExample()
        {
            // Créez un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B5"].PutValue(20);
            worksheet.Cells["B8"].PutValue(50);
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C7"].PutValue(15);
            worksheet.Cells["C9"].PutValue(30);

            // Créer une zone de cellules
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 10;
            ca.StartColumn = 0;
            ca.EndColumn = 10;

            // Ajouter une règle de mise en forme conditionnelle à la feuille de calcul
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "5", "30");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Enregistrez le classeur
            workbook.Save("CellAreaExample.xlsx");
            workbook.Save("CellAreaExample.pdf");

            // Démontrer la méthode ToString
            Console.WriteLine(ca.ToString());

            // Démontrer la méthode CompareTo
            CellArea ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };
            int comparisonResult = ca.CompareTo(ca2);
            Console.WriteLine($"Comparison result: {comparisonResult}");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


