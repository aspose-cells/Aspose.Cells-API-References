---
title: "NameCollection.Add"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode NameCollection. Définit un nouveau nom"
type: docs
url: /fr/net/aspose.cells/namecollection/add/
---
## NameCollection.Add method

Définit un nouveau nom.

```csharp
public int Add(string text)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| texte | String | Le texte à utiliser comme nom. |

### Valeur de retour

[`Name`](../../name/) object index.

### Remarques

Le nom ne peut pas contenir d'espaces et ne doit pas ressembler à des références de cellule.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook(FileFormatType.Xlsx);
            Worksheet worksheet = wb.Worksheets[0];
            
            // Ajoutez un nom avec une référence de chaîne
            int index = wb.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = wb.Worksheets.Names[index];
            
            // Définissez la formule à laquelle le nom fait référence
            namedRange.RefersTo = "=Sheet1!$A$1:$B$10";
            
            // Vérifiez et affichez les résultats
            Console.WriteLine("Named Range RefersTo: " + namedRange.RefersTo);
            Console.WriteLine("Named Range Index: " + index);
            
            // Obtenez la plage et affichez son adresse
            Aspose.Cells.Range range = namedRange.GetRange();
            Console.WriteLine("Range Address: " + range.Address);
        }
    }
}
```

### Voir aussi

* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


