---
title: "WorksheetCollection.Names"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorksheetCollection. Obtient la collection de tous les objets Name dans le classeur"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/names/
---
## WorksheetCollection.Names property

Obtient la collection de tous les objets Name dans le classeur.

```csharp
public NameCollection Names { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyNamesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul avec des caractères spéciaux dans le nom
            Worksheet worksheet = workbook.Worksheets.Add("My.Test");
            
            // Accéder à la collection Names
            NameCollection names = workbook.Worksheets.Names;
            
            // Ajouter une nouvelle plage nommée
            int index = names.Add("My.Test!TestName");
            Name namedRange = names[index];
            
            // Définir la référence de la plage et démontrer son utilisation
            namedRange.RefersTo = "=My.Test!$A$1:$B$2";
            
            // Afficher les propriétés de la plage nommée
            Console.WriteLine("Name: " + namedRange.Text);
            Console.WriteLine("FullText: " + namedRange.FullText);
            Console.WriteLine("RefersTo: " + namedRange.RefersTo);
        }
    }
}
```

### Voir aussi

* class [NameCollection](../../namecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


