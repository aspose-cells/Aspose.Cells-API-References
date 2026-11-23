---
title: "Classe CalculationCell"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.CalculationCell. Représente les données pertinentes de calcul concernant une cellule qui est en cours de calcul"
type: docs
url: /fr/net/aspose.cells/calculationcell/
---
## CalculationCell class

Représente les données pertinentes du calcul concernant une cellule en cours de calcul.

```csharp
public class CalculationCell
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Cell](../../aspose.cells/calculationcell/cell/) { get; } | Obtient l'objet Cell qui est en cours de calcul. |
| [CellColumn](../../aspose.cells/calculationcell/cellcolumn/) { get; } | Obtient l'index de colonne de la cellule. |
| [CellRow](../../aspose.cells/calculationcell/cellrow/) { get; } | Obtient l'index de ligne de la cellule. |
| [Workbook](../../aspose.cells/calculationcell/workbook/) { get; } | Obtient l'objet Workbook. |
| [Worksheet](../../aspose.cells/calculationcell/worksheet/) { get; } | Obtient l'objet Worksheet où se trouve la cellule. |

## Méthodes

| Nom | Description |
| --- | --- |
| [SetCalculatedValue](../../aspose.cells/calculationcell/setcalculatedvalue/)(object) | Définit la valeur calculée pour la cellule. |

### Remarques

L'utilisateur ne doit pas modifier les données du Workbook pendant le processus de calcul de formule, sinon un résultat inattendu ou une exception peut survenir. Ainsi, tous les objets fournis par cette classe (comme l'objet Cell de [`Cell`](./cell/)) sont destinés uniquement à "lecture".

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CellsClassCalculationCellDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Créer une instance de CalculationCell en utilisant la réflexion puisque le constructeur n'est pas public.
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell),
                    BindingFlags.NonPublic | BindingFlags.Instance,
                    null,
                    new object[] { workbook, worksheet, 0, 1, worksheet.Cells["B1"] },
                    null);

                // Afficher les propriétés de base
                Console.WriteLine($"Cell Row: {calcCell.CellRow}");
                Console.WriteLine($"Cell Column: {calcCell.CellColumn}");
                Console.WriteLine($"Cell Value: {calcCell.Cell.Value}");
                Console.WriteLine($"Workbook Name: {calcCell.Workbook.FileName}");
                Console.WriteLine($"Worksheet Name: {calcCell.Worksheet.Name}");

                // Enregistrez le classeur
                workbook.Save("CalculationCellDemo.xlsx");
                Console.WriteLine("CalculationCell demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


