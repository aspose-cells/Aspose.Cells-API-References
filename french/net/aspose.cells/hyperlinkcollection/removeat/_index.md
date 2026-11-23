---
title: "HyperlinkCollection.RemoveAt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode HyperlinkCollection. Supprime le lien hypertexte à l'index spécifié dans cette collection"
type: docs
url: /fr/net/aspose.cells/hyperlinkcollection/removeat/
---
## HyperlinkCollection.RemoveAt method

Supprime le lien hypertexte à l'index spécifié dans cette collection.

```csharp
public void RemoveAt(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | L'indice à base zéro de l'élément. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter un lien hypertexte à la cellule A1
            sheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Vérifier que le lien hypertexte existe avant la suppression
            Console.WriteLine("Hyperlinks count before removal: " + sheet.Hyperlinks.Count);
            
            // Supprime le lien hypertexte à l'index 0
            sheet.Hyperlinks.RemoveAt(0);
            
            // Vérifier que le lien hypertexte a été supprimé
            Console.WriteLine("Hyperlinks count after removal: " + sheet.Hyperlinks.Count);
        }
    }
}
```

### Voir aussi

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


