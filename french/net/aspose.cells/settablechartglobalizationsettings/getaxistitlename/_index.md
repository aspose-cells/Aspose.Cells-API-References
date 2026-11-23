---
title: "SettableChartGlobalizationSettings.GetAxisTitleName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableChartGlobalizationSettings. Obtient le nom du titre pour l'axe"
type: docs
url: /fr/net/aspose.cells/settablechartglobalizationsettings/getaxistitlename/
---
## SettableChartGlobalizationSettings.GetAxisTitleName method

Obtient le nom du Title pour l'axe

```csharp
public override string GetAxisTitleName()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetAxisTitleNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données minimales pour le contexte
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            try
            {
                // Créer une instance de SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Définir un nom de titre d'axe personnalisé
                settings.SetAxisTitleName("Custom Axis Title");

                // Obtenir le nom du titre d'axe en utilisant GetAxisTitleName
                string axisTitleName = settings.GetAxisTitleName();
                Console.WriteLine("Axis Title Name: " + axisTitleName);

                // Enregistrez le classeur
                workbook.Save("GetAxisTitleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetAxisTitleName: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


