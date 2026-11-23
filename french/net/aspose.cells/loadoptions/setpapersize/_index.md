---
title: "LoadOptions.SetPaperSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "LoadOptions method. Définit la taille de papier d’impression par défaut à partir des paramètres de l’imprimante par défaut"
type: docs
url: /fr/net/aspose.cells/loadoptions/setpapersize/
---
## LoadOptions.SetPaperSize method

Définit la taille de papier d'impression par défaut à partir des paramètres de l'imprimante par défaut.

```csharp
public void SetPaperSize(PaperSizeType type)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| type | PaperSizeType | La taille de papier par défaut. |

### Remarques

S'il n'y a aucun paramètre concernant la taille du papier, MS Excel utilisera les paramètres de l'imprimante par défaut.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsMethodSetPaperSizeWithPaperSizeTypeDemo
    {
        public static void Run()
        {
            // Créer des options de chargement et définir la taille du papier à A5
            LoadOptions options = new LoadOptions();
            options.SetPaperSize(PaperSizeType.PaperA5);

            // Charger le classeur avec les options spécifiées
            Workbook workbook = new Workbook("example.xlsx", options);
            
            // Vérifier que la taille du papier est correctement définie
            Console.WriteLine("Paper size of first worksheet: " + workbook.Worksheets[0].PageSetup.PaperSize);
        }
    }
}
```

### Voir aussi

* enum [PaperSizeType](../../papersizetype/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


