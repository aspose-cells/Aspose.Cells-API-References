---
title: "SettablePivotGlobalizationSettings.GetTextOfProtectedName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettablePivotGlobalizationSettings. Obtient le texte pour le nom protégé spécifié"
type: docs
url: /fr/net/aspose.cells/settablepivotglobalizationsettings/gettextofprotectedname/
---
## SettablePivotGlobalizationSettings.GetTextOfProtectedName method

Obtient le texte pour le nom protégé spécifié.

```csharp
public override string GetTextOfProtectedName(string protectedName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| protectedName | String | Le nom protégé dans le tableau croisé dynamique. |

### Valeur de retour

Les noms protégés locaux du tableau croisé dynamique.

### Remarques

Dans Ms Excel, certains noms ne sont pas autorisés à être utilisés comme nom de PivotFields dans le tableau croisé dynamique. Ils diffèrent selon les régions ; l'utilisateur peut les spécifier explicitement en fonction de la région utilisée.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfProtectedNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter quelques données d'exemple pour le contexte
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Créer une instance de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Définir un texte personnalisé pour un nom protégé
                settings.SetTextOfProtectedName("Sum", "Total Sum");

                // Obtenir le texte du nom protégé
                string protectedNameText = settings.GetTextOfProtectedName("Sum");

                Console.WriteLine($"Text for protected name 'Sum': {protectedNameText}");

                // Enregistrez le classeur
                workbook.Save("GetTextOfProtectedNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


