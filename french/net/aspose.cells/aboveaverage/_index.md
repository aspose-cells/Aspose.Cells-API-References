---
title: "Classe AboveAverage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.AboveAverage. Décrivez la règle de mise en forme conditionnelle AboveAverage. Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui sont au-dessus ou en dessous de la moyenne pour toutes les valeurs de la plage."
type: docs
url: /fr/net/aspose.cells/aboveaverage/
---
## AboveAverage class

Décrivez la règle de mise en forme conditionnelle AboveAverage. Cette règle de mise en forme conditionnelle met en surbrillance les cellules qui sont au-dessus ou en dessous de la moyenne pour toutes les valeurs de la plage.

```csharp
public class AboveAverage
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [AboveAverage](aboveaverage/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [IsAboveAverage](../../aspose.cells/aboveaverage/isaboveaverage/) { get; set; } | Obtenez ou définissez le drapeau indiquant si la règle est une règle « au‑dessus de la moyenne ». 'true' indique « au‑dessus de la moyenne ». La valeur par défaut est true. |
| [IsEqualAverage](../../aspose.cells/aboveaverage/isequalaverage/) { get; set; } | Obtenez ou définissez le drapeau indiquant si les critères 'aboveAverage' et 'belowAverage' sont inclusifs de la moyenne elle‑même, ou exclusifs de cette valeur. 'true' indique d’inclure la valeur moyenne dans les critères. La valeur par défaut est false. |
| [StdDev](../../aspose.cells/aboveaverage/stddev/) { get; set; } | Obtenez ou définissez le nombre d'écarts‑type à inclure au‑dessus ou en dessous de la moyenne dans la règle de mise en forme conditionnelle. La valeur d'entrée doit être comprise entre 0 et 3 (inclure 0 et 3). Régler cette valeur à 0 signifie que stdDev n'est pas défini. La valeur par défaut est 0. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class AboveAverageDemo
    {
        public static void AboveAverageExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            // Ajouter une collection de mise en forme conditionnelle à la feuille de calcul
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            // Définir la zone de cellules où appliquer la mise en forme conditionnelle
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Ajouter une condition au‑dessus de la moyenne à la collection
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            // Définir la couleur d'arrière‑plan pour la condition
            fc.Style.BackgroundColor = Color.Yellow;

            // Définir les propriétés pour la condition au‑dessus de la moyenne
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            Cells cells = worksheet.Cells;
            cells["A1"].Value = 20;
            cells["A2"].Value = 300;
            cells["A3"].Value = 40;
            cells["A4"].Value = 500;
            cells["A5"].Value = 6;
            cells["A6"].Value = 70;
            cells["A7"].Value = 8;
            cells["A8"].Value = 900;
            cells["A9"].Value = 10;

            cells["C1"].Value = 2;
            cells["C2"].Value = 3;
            cells["C3"].Value = 4;
            cells["C4"].Value = 5;
            cells["C5"].Value = 3;
            cells["C6"].Value = 2;
            cells["C7"].Value = 8;
            cells["C8"].Value = 300;
            cells["C9"].Value = 10;

            // Enregistrez le classeur
            workbook.Save("AboveAverageExample.xlsx");
            workbook.Save("AboveAverageExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


