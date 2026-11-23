---
title: "SettableGlobalizationSettings.SetTableRowTypeOfHeaders"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Définit le nom du type des lignes de tableau qui constituent l'en-tête du tableau"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/settablerowtypeofheaders/
---
## SettableGlobalizationSettings.SetTableRowTypeOfHeaders method

Définit le nom du type des lignes de tableau qui comprennent l'en-tête du tableau.

```csharp
public void SetTableRowTypeOfHeaders(string name)
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

    public class SettableGlobalizationSettingsMethodSetTableRowTypeOfHeadersWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un tableau et ajouter des données
            Cells cells = worksheet.Cells;
            cells["A1"].PutValue("Header1");
            cells["B1"].PutValue("Header2");
            cells["A2"].PutValue("Value1");
            cells["B2"].PutValue("Value2");
            
            // Créer un ListObject (Table)
            int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.ShowTotals = true;

            // Créer une instance de SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Appeler SetTableRowTypeOfHeaders avec un nom de type d'en-tête personnalisé
                settings.SetTableRowTypeOfHeaders("CustomHeaders");

                // Appliquer les paramètres au classeur
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("Table header type name set to: CustomHeaders");
                Console.WriteLine("In formulas, '#CustomHeaders' will now represent the table header");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTableRowTypeOfHeaders method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("SetTableRowTypeOfHeadersDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


