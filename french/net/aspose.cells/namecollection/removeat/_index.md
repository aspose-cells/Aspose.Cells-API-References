---
title: "NameCollection.RemoveAt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode NameCollection. Supprime le nom à l'index spécifié"
type: docs
url: /fr/net/aspose.cells/namecollection/removeat/
---
## NameCollection.RemoveAt method

Supprime le nom à l'index spécifique.

```csharp
public void RemoveAt(int index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indice | Int32 | indice du Name à supprimer. |

### Remarques

Veuillez vous assurer que le nom n'est pas référencé par les autres formules avant d'appeler la méthode. Et si le nom est référencé, définir Name.RefersTo à null est préférable.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            WorksheetCollection worksheets = workbook.Worksheets;
            NameCollection names = worksheets.Names;

            // Ajouter des noms à la collection
            int firstIndex = names.Add("FirstRange");
            names[firstIndex].RefersTo = "=Sheet1!$A$1:$A$5";
            
            int secondIndex = names.Add("SecondRange");
            names[secondIndex].RefersTo = "=Sheet1!$B$1:$B$5";

            // Supprimer le nom par indice
            names.RemoveAt(firstIndex);

            // Vérifier la suppression en vérifiant le nombre
            Console.WriteLine($"Remaining names count: {names.Count}");

            workbook.Save("NameCollectionRemoveAtExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


