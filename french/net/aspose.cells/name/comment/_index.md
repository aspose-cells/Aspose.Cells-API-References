---
title: "Name.Comment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Name. Obtient et définit le commentaire du nom. S'applique uniquement aux versions Excel 2007 ou supérieures"
type: docs
url: /fr/net/aspose.cells/name/comment/
---
## Name.Comment property

Obtient et définit le commentaire du nom. S’applique uniquement aux versions Excel 2007 ou supérieures.

```csharp
public string Comment { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyCommentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une plage nommée avec commentaire
            int index = workbook.Worksheets.Names.Add("TestRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$B$2";
            namedRange.Comment = "This is a test named range";
            
            // Enregistrez le classeur
            workbook.Save("NamedRangeWithComment.xlsx");
            
            // Charger le classeur enregistré pour vérifier le commentaire
            Workbook loadedWorkbook = new Workbook("NamedRangeWithComment.xlsx");
            Name loadedNamedRange = loadedWorkbook.Worksheets.Names[0];
            
            // Afficher le commentaire pour démontrer la fonctionnalité
            Console.WriteLine("Named Range Comment: " + loadedNamedRange.Comment);
        }
    }
}
```

### Voir aussi

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


