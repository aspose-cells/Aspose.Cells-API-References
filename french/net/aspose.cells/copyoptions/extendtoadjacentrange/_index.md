---
title: "CopyOptions.ExtendToAdjacentRange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CopyOptions. Indique s'il faut étendre les plages lors de la copie de la plage vers une plage adjacente"
type: docs
url: /fr/net/aspose.cells/copyoptions/extendtoadjacentrange/
---
## CopyOptions.ExtendToAdjacentRange property

Indique s'il faut étendre les plages lors de la copie de la plage vers la plage adjacente.

```csharp
public bool ExtendToAdjacentRange { get; set; }
```

### Remarques

Si c'est true, cela n'étend que la plage du lien hypertexte, sans ajouter de nouveau lien hypertexte lors de la copie des liens hypertexte vers des lignes adjacentes.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyExtendToAdjacentRangeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Ajouter un lien hypertexte à la cellule A1
            ws.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Créer des options de copie et définir ExtendToAdjacentRange sur true
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.ExtendToAdjacentRange = true;

            // Copier la ligne 0 vers la ligne 1 avec les options de copie
            ws.Cells.CopyRows(ws.Cells, 0, 1, 1, copyOptions);

            // Vérifier que le lien hypertexte a été étendu à la plage adjacente
            Console.WriteLine("Hyperlink count after copy: " + ws.Hyperlinks.Count);
        }
    }
}
```

### Voir aussi

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


