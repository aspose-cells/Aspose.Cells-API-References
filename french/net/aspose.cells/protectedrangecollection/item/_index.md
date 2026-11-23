---
title: "ProtectedRangeCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ProtectedRangeCollection. Obtient l'élément ProtectedRange à l'indice spécifié"
type: docs
url: /fr/net/aspose.cells/protectedrangecollection/item/
---
## ProtectedRangeCollection indexer

Obtient l'élément [`ProtectedRange`](../../protectedrange/) à l'indice spécifié.

```csharp
public ProtectedRange this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une plage protégée en utilisant les indices de cellules (startRow, startColumn, endRow, endColumn)
            int index = worksheet.AllowEditRanges.Add("MyProtectedRange", 0, 0, 1, 1);
            ProtectedRange protectedRange = worksheet.AllowEditRanges[index];
            protectedRange.Password = "password123";
            
            // Accéder à la plage protégée en utilisant la propriété Item (indice 0)
            ProtectedRange retrievedRange = worksheet.AllowEditRanges[0];
            
            // Vérifier et afficher l'état de protection
            Console.WriteLine("Is protected with password: " + retrievedRange.IsProtectedWithPassword);
            Console.WriteLine("Range name: " + retrievedRange.Name);
            
            // Enregistrez le classeur
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ProtectedRange](../../protectedrange/)
* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


