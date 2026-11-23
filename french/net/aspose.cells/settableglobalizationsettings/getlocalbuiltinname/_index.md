---
title: "SettableGlobalizationSettings.GetLocalBuiltInName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode SettableGlobalizationSettings. Obtient le texte dépendant de la locale pour le built-in Name selon le texte standard fourni"
type: docs
url: /fr/net/aspose.cells/settableglobalizationsettings/getlocalbuiltinname/
---
## SettableGlobalizationSettings.GetLocalBuiltInName method

Obtient le texte dépendant de la langue pour le nom intégré selon le texte standard fourni.

```csharp
public override string GetLocalBuiltInName(string standardName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| standardName | String | Texte Standard (locale en-US) du built-in Name. |

### Valeur de retour

Texte dépendant de la locale. La locale a été spécifiée par le classeur pour lequel ces paramètres sont utilisés.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetLocalBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez une instance de SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // Appeler la méthode GetLocalBuiltInName avec un nom intégré standard
                string standardName = "SUM";
                string localName = globalizationSettings.GetLocalBuiltInName(standardName);

                // Afficher le résultat
                Console.WriteLine($"Standard name: {standardName}, Local name: {localName}");

                // Définir un nom local personnalisé pour le nom intégré standard
                globalizationSettings.SetLocalBuiltInName(standardName, "CustomSum", true);

                // Obtenir à nouveau le nom local après l'avoir défini
                localName = globalizationSettings.GetLocalBuiltInName(standardName);
                Console.WriteLine($"After setting - Standard name: {standardName}, Local name: {localName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalBuiltInName method: {ex.Message}");
            }

            // Enregistrez le classeur
            workbook.Save("MethodGetLocalBuiltInNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


