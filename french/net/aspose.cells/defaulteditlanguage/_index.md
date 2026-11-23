---
title: "Enum DefaultEditLanguage"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.DefaultEditLanguage enum. Représente la langue d'édition par défaut"
type: docs
url: /fr/net/aspose.cells/defaulteditlanguage/
---
## DefaultEditLanguage enumeration

Représente la langue d'édition par défaut.

```csharp
public enum DefaultEditLanguage
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Auto | `0` | Représente la détection automatique de la langue d'édition en fonction du texte lui‑même. |
| English | `1` | Représente la langue anglaise. |
| CJK | `2` | Représente les langues chinoise, japonaise et coréenne. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DefaultEditLanguageDemo
    {
        public static void DefaultEditLanguageExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez AutoFitterOptions et définissez DefaultEditLanguage
            AutoFitterOptions autoFitterOptions = new AutoFitterOptions();
            autoFitterOptions.DefaultEditLanguage = DefaultEditLanguage.CJK;

            // Appliquez l'ajustement automatique des lignes avec les options spécifiées
            worksheet.AutoFitRows(autoFitterOptions);

            // Enregistrez le classeur
            workbook.Save("DefaultEditLanguageExample.xlsx");
            workbook.Save("DefaultEditLanguageExample.pdf");

            // Affichez le DefaultEditLanguage défini dans la console
            Console.WriteLine("Default Edit Language set to: " + autoFitterOptions.DefaultEditLanguage);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


