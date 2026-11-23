---
title: "HorizontalPageBreak.EndColumn"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété HorizontalPageBreak. Obtient l'index de la colonne de fin de cette rupture de page horizontale"
type: docs
url: /fr/net/aspose.cells/horizontalpagebreak/endcolumn/
---
## HorizontalPageBreak.EndColumn property

Obtient l'indice de colonne de fin de ce saut de page horizontal.

```csharp
public int EndColumn { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyEndColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une rupture de page horizontale à la ligne 5, s'étendant de la colonne 2 à 4
            int index = worksheet.HorizontalPageBreaks.Add(5, 2, 4);
            HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];

            // Affichez la propriété EndColumn
            Console.WriteLine("Horizontal Page Break EndColumn: " + hPageBreak.EndColumn);

            // Étant donné que EndColumn est en lecture seule, nous devons supprimer et réajouter la rupture de page pour la modifier
            worksheet.HorizontalPageBreaks.RemoveAt(index);
            index = worksheet.HorizontalPageBreaks.Add(5, 2, 6);
            hPageBreak = worksheet.HorizontalPageBreaks[index];
            Console.WriteLine("Modified Horizontal Page Break EndColumn: " + hPageBreak.EndColumn);
        }
    }
}
```

### Voir aussi

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


