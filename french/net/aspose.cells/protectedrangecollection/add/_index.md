---
title: "ProtectedRangeCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ProtectedRangeCollection. Ajoute un élément ProtectedRange à la collection"
type: docs
url: /fr/net/aspose.cells/protectedrangecollection/add/
---
## ProtectedRangeCollection.Add method

Ajoute un élément [`ProtectedRange`](../../protectedrange/) à la collection.

```csharp
public int Add(string name, int startRow, int startColumn, int endRow, int endColumn)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Titre de la plage. Ceci est utilisé comme un descripteur, pas comme une définition de plage nommée. |
| startRow | Int32 | Indice de ligne de départ de la plage. |
| startColumn | Int32 | Indice de colonne de départ de la plage. |
| endRow | Int32 | Indice de ligne de fin de la plage. |
| endColumn | Int32 | Indice de colonne de fin de la plage. |

### Valeur de retour

indice d'objet.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangeCollectionMethodAddWithStringInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            ProtectedRangeCollection pranges = workbook.Worksheets[0].AllowEditRanges;
            
            // Ajouter une plage protégée avec un nom et des coordonnées
            int index = pranges.Add("Range1", 0, 0, 10, 10);
            
            // Accéder à la plage ajoutée
            ProtectedRange range = pranges[index];
            
            // Définir le descripteur de sécurité
            string securityDescriptor = "O:WDG:WDD:(D;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1000)(A;;CC;;;S-1-5-21-2854911246-2539335229-2923752399-1013)";
            range.SecurityDescriptor = securityDescriptor;
            
            // Enregistrer et vérifier
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [ProtectedRangeCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


