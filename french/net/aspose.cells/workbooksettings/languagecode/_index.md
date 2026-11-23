---
title: "WorkbookSettings.LanguageCode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorkbookSettings. Obtient ou définit la langue de l'interface utilisateur de la version du classeur en fonction du CountryCode qui a enregistré le fichier"
type: docs
url: /fr/net/aspose.cells/workbooksettings/languagecode/
---
## WorkbookSettings.LanguageCode property

Obtient ou définit la langue de l'interface utilisateur de la version du classeur basée sur le CountryCode qui a enregistré le fichier.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux paramètres du classeur
            WorkbookSettings settings = workbook.Settings;

            // Définir le code langue sur Allemand (Allemagne)
            settings.LanguageCode = CountryCode.Germany;

            // Afficher le code langue actuel
            Console.WriteLine("Current Language Code: " + settings.LanguageCode);

            // Modifier le code langue en Français (France)
            settings.LanguageCode = CountryCode.France;
            Console.WriteLine("Updated Language Code: " + settings.LanguageCode);

            // Enregistrez le classeur
            workbook.Save("WorkbookSettings_LanguageCodeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


