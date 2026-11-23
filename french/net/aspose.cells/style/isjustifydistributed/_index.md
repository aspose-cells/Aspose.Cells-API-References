---
title: "Style.IsJustifyDistributed"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Indique si l'alignement justifié ou distribué des cellules doit être utilisé sur la dernière ligne de texte"
type: docs
url: /fr/net/aspose.cells/style/isjustifydistributed/
---
## Style.IsJustifyDistributed property

Indique si l'alignement justifié ou réparti des cellules doit être utilisé sur la dernière ligne de texte.

```csharp
public bool IsJustifyDistributed { get; set; }
```

### Remarques

Ceci est typique pour les alignements d'Asie de l'Est mais pas typique dans d'autres contextes. Ne fonctionne que lorsque l'alignement distribué est utilisé.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsJustifyDistributedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la cellule B3 et définir son texte
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("Sample Text");

            // Obtenir le style de la cellule et définir IsJustifyDistributed sur true
            Style style = cell.GetStyle();
            style.IsJustifyDistributed = true;
            cell.SetStyle(style);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");

            // Vérifier la propriété
            Console.WriteLine("IsJustifyDistributed: " + cell.GetStyle().IsJustifyDistributed);
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


