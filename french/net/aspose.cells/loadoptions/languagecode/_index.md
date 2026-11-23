---
title: "LoadOptions.LanguageCode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Obtient ou définit la langue de l'interface utilisateur de la version du Workbook basée sur le CountryCode qui a enregistré le fichier"
type: docs
url: /fr/net/aspose.cells/loadoptions/languagecode/
---
## LoadOptions.LanguageCode property

Obtient ou définit la langue de l'interface utilisateur de la version du classeur basée sur le CountryCode qui a enregistré le fichier.

```csharp
public CountryCode LanguageCode { get; set; }
```

### Exemples

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // Créez une instance de LoadOptions
            LoadOptions loadOptions = new LoadOptions();

            // Définir la propriété LanguageCode
            loadOptions.LanguageCode = CountryCode.USA;

            // Charger un classeur avec les LoadOptions spécifiés
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);

            // Accéder à la feuille de calcul et modifier le contenu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Language Code Demo");

            // Enregistrer le classeur modifié
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


