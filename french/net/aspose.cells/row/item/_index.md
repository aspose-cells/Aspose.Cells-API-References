---
title: "Row.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Row. Obtient la cellule"
type: docs
url: /fr/net/aspose.cells/row/item/
---
## Row indexer

Obtient la cellule.

```csharp
public Cell this[int column] { get; }
```

| Paramètre | Description |
| --- | --- |
| column | L'index de colonne |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Accéder à la première ligne
            Row row = sheet.Cells.Rows[0];
            
            // Définir le contenu HTML avec différents styles de couleur
            row[0].HtmlString = @"<span style=""color:#ffAb68;"">TEST</span>";
            row[1].HtmlString = @"<span style=""color:inherit;"">TEST</span>";
            
            // Démontrer l'utilisation de la propriété Item et afficher les couleurs
            Console.WriteLine("Cell 0 Font Color: " + row[0].GetStyle().Font.Color.Name);
            Console.WriteLine("Cell 1 Font Color: " + row[1].GetStyle().Font.Color.Name);
        }
    }
}
```

### Voir aussi

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


