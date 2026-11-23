---
title: "GlobalizationSettings.GetTableRowTypeOfCurrent"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GlobalizationSettings. Obtient le nom du type des lignes de tableau qui comprend la ligne actuelle dans la table référencée. La valeur par défaut est This Row, donc dans la formule This Row représente la ligne actuelle dans la table référencée"
type: docs
url: /fr/net/aspose.cells/globalizationsettings/gettablerowtypeofcurrent/
---
## GlobalizationSettings.GetTableRowTypeOfCurrent method

Obtient le nom du type de lignes de tableau qui comprend la ligne actuelle du tableau référencé. La valeur par défaut est "This Row", ainsi dans la formule "#This Row" représente la ligne actuelle du tableau référencé.

```csharp
public virtual string GetTableRowTypeOfCurrent()
```

### Valeur de retour

le nom du type des lignes de tableau

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class GlobalizationSettingsMethodGetTableRowTypeOfCurrentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir des paramètres de globalisation personnalisés
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // Créez des données d'exemple et un tableau
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(2.5);
                worksheet.Cells["A3"].PutValue("Orange");
                worksheet.Cells["B3"].PutValue(1.8);

                // Créez un tableau
                int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
                ListObject table = worksheet.ListObjects[tableIndex];
                table.DisplayName = "PriceTable"; // Fixed property name

                // Ajoutez une formule en utilisant la référence de la ligne actuelle
                Cell formulaCell = worksheet.Cells["C2"];
                formulaCell.Formula = "=PriceTable[@Price] * 1.2";

                // Démontrez l'effet de GetTableRowTypeOfCurrent
                Console.WriteLine("Generated formula: " + formulaCell.Formula);
                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfCurrent method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("MethodGetTableRowTypeOfCurrentDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetTableRowTypeOfCurrent()
        {
            return "CurrentItem"; // Custom current row identifier
        }
    }
}
```

### Voir aussi

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


