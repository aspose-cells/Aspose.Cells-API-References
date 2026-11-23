---
title: "SettableGlobalizationSettings.SetTableRowTypeOfAll"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Définit le nom du type des lignes de tableau qui comprend toutes les lignes dans la table référencée"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/settablerowtypeofall/
---
## SettableGlobalizationSettings.SetTableRowTypeOfAll method

Définit le nom du type des lignes de tableau qui comprennent toutes les lignes du tableau référencé.

```csharp
public void SetTableRowTypeOfAll(string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | le nom du type des lignes de tableau |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfAllWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez des données d'exemple pour un tableau
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Product");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(2.5);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(1.8);

            // Créer un tableau
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            // Créer des paramètres de mondialisation personnalisés
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Appelez SetTableRowTypeOfAll avec un nom personnalisé
                settings.SetTableRowTypeOfAll("CompleteTable");

                // Appliquer les paramètres au classeur
                workbook.Settings.GlobalizationSettings = settings;

                // Vérifiez le paramètre en récupérant la valeur
                string rowType = settings.GetTableRowTypeOfAll();
                Console.WriteLine($"Table row type for all rows set to: {rowType}");

                // Ajouter une formule qui référence toutes les lignes en utilisant le nom personnalisé
                cells["C2"].Formula = "=SUM(#CompleteTable[Price])";
                Console.WriteLine($"Formula using custom row type: {cells["C2"].Formula}");

                // Calculer les formules
                workbook.CalculateFormula();
                Console.WriteLine($"Calculation result: {cells["C2"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfAll method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("MethodSetTableRowTypeOfAllWithStringDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


