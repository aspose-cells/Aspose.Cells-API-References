---
title: "LoadOptions.AutoFilter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Indique si le filtrage automatique des données est appliqué lors du chargement des fichiers"
type: docs
url: /fr/net/aspose.cells/loadoptions/autofilter/
---
## LoadOptions.AutoFilter property

Indique si le filtrage automatique des données est appliqué lors du chargement des fichiers.

```csharp
public bool AutoFilter { get; set; }
```

### Remarques

Parfois, même si autofilter est activé, les lignes correspondantes ne sont pas masquées dans le fichier. Cela ne fonctionne maintenant que pour les fichiers SpreadSheetML.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Créer des options de chargement et activer AutoFilter
            LoadOptions options = new LoadOptions();
            options.AutoFilter = true;

            // Charger le classeur avec AutoFilter activé
            Workbook workbook = new Workbook("example.xlsx", options);

            // Accéder à la première feuille de calcul et appliquer AutoFilter
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.AutoFilter.Range = "A1:D10";
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


