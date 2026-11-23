---
title: "CalculationCell.SetCalculatedValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CalculationCell. Définit la valeur calculée pour la cellule"
type: docs
url: /fr/net/aspose.cells/calculationcell/setcalculatedvalue/
---
## CalculationCell.SetCalculatedValue method

Définit la valeur calculée pour la cellule.

```csharp
public void SetCalculatedValue(object v)
```

### Remarques

L'utilisateur peut définir le résultat calculé avec cette méthode pour ignorer le calcul automatique de la cellule.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellMethodSetCalculatedValueWithObjectDemo
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

                // Définir une valeur calculée en utilisant la méthode SetCalculatedValue
                calcCell.SetCalculatedValue(42); // Using an integer value as the Object parameter

                // Afficher les informations sur la cellule
                Console.WriteLine("Cell Row: " + calcCell.CellRow);
                Console.WriteLine("Cell Column: " + calcCell.CellColumn);
                Console.WriteLine("SetCalculatedValue method called successfully with value: 42");

                // Enregistrez le classeur
                workbook.Save("SetCalculatedValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetCalculatedValue: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


