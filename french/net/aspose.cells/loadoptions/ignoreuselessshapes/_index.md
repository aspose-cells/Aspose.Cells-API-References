---
title: "LoadOptions.IgnoreUselessShapes"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "LoadOptions property. Indique si les formes inutiles sont ignorées"
type: docs
url: /fr/net/aspose.cells/loadoptions/ignoreuselessshapes/
---
## LoadOptions.IgnoreUselessShapes property

Indique s'il faut ignorer les formes inutiles.

```csharp
public bool IgnoreUselessShapes { get; set; }
```

### Remarques

Fonctionne uniquement pour les fichiers xlsx, xlsb et xlsm. Il existe de nombreuses formes identiques qui se chevauchent et qui sont inutiles dans certains fichiers ; nous pouvons les ignorer lors du chargement des fichiers.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyIgnoreUselessShapesDemo
    {
        public static void Run()
        {
            // Créer des options de chargement et définir IgnoreUselessShapes sur true
            LoadOptions options = new LoadOptions();
            options.IgnoreUselessShapes = true;

            // Chargez le classeur avec les options
            Workbook workbook = new Workbook("example.xlsx", options);

            // Afficher le nombre de formes dans la première feuille de calcul
            Console.WriteLine("Shapes count: " + workbook.Worksheets[0].Shapes.Count);
        }
    }
}
```

### Voir aussi

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


