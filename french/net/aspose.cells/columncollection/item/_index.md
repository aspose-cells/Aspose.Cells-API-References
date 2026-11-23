---
title: "ColumnCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ColumnCollection propriété. Obtient un objet Column par indice de colonne. L'objet Column de l'indice de colonne donné sera instancié s'il n'existe pas auparavant"
type: docs
url: /fr/net/aspose.cells/columncollection/item/
---
## ColumnCollection indexer

Obtient un [`Column`](../../column/) objet par indice de colonne. L'objet Column de l'indice de colonne donné sera instancié s'il n'existe pas auparavant.

```csharp
public Column this[int columnIndex] { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à la collection de colonnes
            ColumnCollection columns = worksheet.Cells.Columns;
            
            // Définir la largeur des colonnes en utilisant la propriété Item
            columns[0].Width = 10;
            columns[1].Width = 15;
            columns[2].Width = 20;
            
            // Afficher les largeurs des colonnes
            Console.WriteLine("Column 0 Width: " + columns[0].Width);
            Console.WriteLine("Column 1 Width: " + columns[1].Width);
            Console.WriteLine("Column 2 Width: " + columns[2].Width);
            
            // Vérifier que les largeurs de colonnes sont définies correctement
            if (columns[0].Width != 10 || columns[1].Width != 15 || columns[2].Width != 20)
            {
                throw new Exception("Column widths were not set correctly");
            }
        }
    }
}
```

### Voir aussi

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


