---
title: "CalculationCell.CellColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CalculationCell. Obtient l'index de colonne de la cellule"
type: docs
url: /fr/net/aspose.cells/calculationcell/cellcolumn/
---
## CalculationCell.CellColumn property

Obtient l'index de colonne de la cellule.

```csharp
public int CellColumn { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationCellPropertyCellColumnDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur et obtenez la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Insérer des données et une formule simple
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Obtenir une instance de CalculationCell via la réflexion (son constructeur est non public)
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell), 
                    nonPublic: true);

                // Lire et afficher la valeur de la propriété CellColumn
                Console.WriteLine("CellColumn value: " + calcCell.CellColumn);

                // Démonstration supplémentaire des propriétés associées (optionnel)
                Console.WriteLine("CellRow value: " + calcCell.CellRow);
                Console.WriteLine("Workbook is null: " + (calcCell.Workbook == null));
                Console.WriteLine("Worksheet is null: " + (calcCell.Worksheet == null));

                // Enregistrer le Workbook (le fichier contiendra les données que nous avons ajoutées)
                workbook.Save("CellColumnDemo.xlsx");
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


