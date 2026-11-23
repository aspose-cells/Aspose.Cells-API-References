---
title: "HighlightChangesOptions.HighlightChangesOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur HighlightChangesOptions. Représente les options de mise en évidence des révisions ou des modifications de fichiers Excel partagés"
type: docs
url: /fr/net/aspose.cells.revisions/highlightchangesoptions/highlightchangesoptions/
---
## HighlightChangesOptions constructor

Représente les options de mise en évidence des révisions ou des modifications des fichiers Excel partagés.

```csharp
public HighlightChangesOptions(bool highlightOnScreen, bool listOnNewSheet)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| highlightOnScreen | Boolean | Indique si la mise en évidence des modifications à l'écran est activée. |
| listOnNewSheet | Boolean | Indique si la liste des modifications sur une nouvelle feuille de calcul est activée. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class HighlightChangesOptionsMethodCtorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A2"].PutValue(100);
            
            // Créer HighlightChangesOptions avec des paramètres booléens
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);
            
            // Simuler le suivi des modifications (normalement vous auriez des révisions réelles)
            Console.WriteLine("HighlightChangesOptions created with:");
            Console.WriteLine($"First parameter (show changes): {true}");
            Console.WriteLine($"Second parameter (changes on new sheet): {true}");
            
            // Enregistrez le classeur
            workbook.Save("HighlightChangesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [HighlightChangesOptions](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


