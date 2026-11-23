---
title: "LoadOptions.KeepUnparsedData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LoadOptions. Indique s’il faut conserver les données non analysées en mémoire pour le classeur lorsqu’il est chargé à partir du fichier modèle. La valeur par défaut est true"
type: docs
url: /fr/net/aspose.cells/loadoptions/keepunparseddata/
---
## LoadOptions.KeepUnparsedData property

Indique s'il faut conserver les données non analysées en mémoire pour le Workbook lorsqu'il est chargé à partir d'un fichier modèle. La valeur par défaut est vraie.

```csharp
public bool KeepUnparsedData { get; set; }
```

### Remarques

Pour les scénarios où l'utilisateur n'a besoin de lire que certains contenus du fichier modèle et n'a pas besoin d'enregistrer le classeur, définir cette propriété sur false peut améliorer les performances, en particulier lorsqu'elle est utilisée avec un type de LoadFilter,

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyKeepUnparsedDataDemo
    {
        public static void Run()
        {
            // Créez des options de chargement et définissez KeepUnparsedData sur false
            LoadOptions options = new LoadOptions();
            options.KeepUnparsedData = false;

            // Charger le classeur avec des options
            Workbook workbook = new Workbook("example.xlsx", options);

            // Accédez à la feuille de calcul et démontrez que les données non analysées ne sont pas conservées
            Worksheet worksheet = workbook.Worksheets[0];
            Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value);

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


