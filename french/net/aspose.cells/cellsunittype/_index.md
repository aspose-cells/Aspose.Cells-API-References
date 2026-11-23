---
title: "Enumération CellsUnitType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enumération Aspose.Cells.CellsUnitType. Spécifie l'unité de mesure"
type: docs
url: /fr/net/aspose.cells/cellsunittype/
---
## CellsUnitType enumeration

Spécifie l'unité de mesure.

```csharp
public enum CellsUnitType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Pixel | `1` | La mesure est en pixels. |
| Point | `2` | La mesure est en points. Un point représente 1/72 de pouce. |
| Inch | `4` | La mesure est en pouces. |
| Cm | `6` | La mesure est en centimètres. |
| Character | `7` | En unité de caractères. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Démontrer l'utilisation de différentes valeurs d'énumération CellsUnitType
                Console.WriteLine("Available CellsUnitType values:");

                // Afficher toutes les valeurs d'énumération
                Console.WriteLine("Pixel: " + CellsUnitType.Pixel);
                Console.WriteLine("Point: " + CellsUnitType.Point);
                Console.WriteLine("Inch: " + CellsUnitType.Inch);
                Console.WriteLine("Cm: " + CellsUnitType.Cm);
                Console.WriteLine("Character: " + CellsUnitType.Character);

                // Exemple d'utilisation : définir la largeur de colonne en utilisant différentes unités
                worksheet.Cells.SetColumnWidthPixel(0, 100); // Using Pixel unit
                worksheet.Cells.SetColumnWidthInch(1, 2.0);  // Using Inch unit

                // Enregistrez le classeur pour démontrer un flux complet
                workbook.Save("CellsUnitTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with different unit types applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with CellsUnitType: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


