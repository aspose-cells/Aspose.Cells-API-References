---
title: "IndividualFontConfigs.IndividualFontConfigs"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur IndividualFontConfigs. Ctor"
type: docs
url: /fr/net/aspose.cells/individualfontconfigs/individualfontconfigs/
---
## IndividualFontConfigs constructor

Constructeur.

```csharp
public IndividualFontConfigs()
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IndividualFontConfigsMethodCtorDemo
    {
        public static void Run()
        {
            // Créer des options de chargement avec IndividualFontConfigs
            var loadOptions = new OdsLoadOptions
            {
                FontConfigs = new IndividualFontConfigs(),
                StandardFont = "Arial",
                StandardFontSize = 12
            };

            // Créer un nouveau classeur avec une feuille de calcul par défaut
            var workbook = new Workbook(FileFormatType.Xlsx);
            
            // Accéder à une feuille de calcul et ajouter du texte
            var worksheet = workbook.Worksheets[0];
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Sample text with custom font configs");

            // Enregistrez le classeur (les options de chargement ne sont pas nécessaires pour l'enregistrement)
            workbook.Save("FontConfigsDemo.ods", SaveFormat.Ods);
        }
    }
}
```

### Voir aussi

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


