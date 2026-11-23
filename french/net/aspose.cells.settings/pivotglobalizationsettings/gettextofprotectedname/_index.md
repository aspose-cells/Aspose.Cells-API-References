---
title: "PivotGlobalizationSettings.GetTextOfProtectedName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PivotGlobalizationSettings. Obtient le texte pour le nom protégé spécifié"
type: docs
url: /fr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofprotectedname/
---
## PivotGlobalizationSettings.GetTextOfProtectedName method

Obtient le texte pour le nom protégé spécifié.

```csharp
public virtual string GetTextOfProtectedName(string protectedName)
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
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfProtectedNameWithStringDemo
    {
        public static void Run()
        {
            try
            {
                // Créer une instance de PivotGlobalizationSettings
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // Définissez un nom protégé pour récupérer son texte
                string protectedName = "SensitiveData";

                // Appelez la méthode GetTextOfProtectedName
                string result = globalizationSettings.GetTextOfProtectedName(protectedName);

                // Afficher le résultat
                Console.WriteLine($"Text for protected name \"{protectedName}\": {result}");
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

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


