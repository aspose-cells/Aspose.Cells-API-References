---
title: "Classe ScenarioInputCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ScenarioInputCell. Représente la cellule d'entrée pour le scénario"
type: docs
url: /fr/net/aspose.cells/scenarioinputcell/
---
## ScenarioInputCell class

Représente la cellule d'entrée pour le scénario.

```csharp
public class ScenarioInputCell
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Column](../../aspose.cells/scenarioinputcell/column/) { get; } | Obtient et définit l'index de colonne de la cellule d'entrée. |
| [IsDeleted](../../aspose.cells/scenarioinputcell/isdeleted/) { get; set; } | Indique si la cellule d'entrée est supprimée. |
| [Name](../../aspose.cells/scenarioinputcell/name/) { get; } | Obtient et définit l'adresse de la cellule d'entrée. |
| [Row](../../aspose.cells/scenarioinputcell/row/) { get; } | Obtient et définit l'index de ligne de la cellule d'entrée. |
| [Value](../../aspose.cells/scenarioinputcell/value/) { get; set; } | Obtient et définit la valeur de la cellule d'entrée. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioInputCellDemo
    {
        public static void ScenarioInputCellExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez un scénario à la feuille de calcul
            int scenarioIndex = worksheet.Scenarios.Add("Scenario 1");
            Scenario scenario = worksheet.Scenarios[scenarioIndex];

            // Ajoutez des cellules d'entrée au scénario
            ScenarioInputCellCollection inputCells = scenario.InputCells;
            inputCells.Add(0, 0, "100"); // Adding cell A1 with value 100
            inputCells.Add(1, 1, "200"); // Adding cell B2 with value 200

            // Accès aux cellules d'entrée
            ScenarioInputCell inputCell1 = inputCells[0];
            ScenarioInputCell inputCell2 = inputCells[1];

            // Affichage des propriétés des cellules d'entrée
            Console.WriteLine($"Input Cell 1: Row = {inputCell1.Row}, Column = {inputCell1.Column}, Value = {inputCell1.Value}, IsDeleted = {inputCell1.IsDeleted}");
            Console.WriteLine($"Input Cell 2: Row = {inputCell2.Row}, Column = {inputCell2.Column}, Value = {inputCell2.Value}, IsDeleted = {inputCell2.IsDeleted}");

            // Modifiez la valeur de la première cellule d'entrée
            inputCell1.Value = "150";

            // Enregistrez le classeur
            workbook.Save("ScenarioInputCellExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


