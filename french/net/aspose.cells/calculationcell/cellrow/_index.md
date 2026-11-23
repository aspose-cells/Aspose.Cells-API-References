---
title: "CalculationCell.CellRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CalculationCell. Obtient l'indice de ligne de la cellule"
type: docs
url: /fr/net/aspose.cells/calculationcell/cellrow/
---
## CalculationCell.CellRow property

Obtient l'index de ligne de la cellule.

```csharp
public int CellRow { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyCellRowDemo
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

                // Affiche la valeur de la propriété CellRow
                Console.WriteLine("CellRow value: " + calcCell.CellRow);

                // Démontrez les propriétés liées pour le contexte
                Console.WriteLine("CellColumn value: " + calcCell.CellColumn);
                Console.WriteLine("Cell Value: " + calcCell.Cell.Value);

                // Enregistrez le classeur
                workbook.Save("CellRowDemo.xlsx");
                Console.WriteLine("CellRow property demonstration completed successfully.");
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

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


