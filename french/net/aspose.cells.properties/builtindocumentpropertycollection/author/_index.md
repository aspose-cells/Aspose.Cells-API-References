---
title: "BuiltInDocumentPropertyCollection.Author"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BuiltInDocumentPropertyCollection. Obtient ou définit le nom de l'auteur du document"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/author/
---
## BuiltInDocumentPropertyCollection.Author property

Obtient ou définit le nom de l'auteur du document.

```csharp
public string Author { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyAuthorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Définir la propriété author
            string authorName = "John Doe";
            workbook.BuiltInDocumentProperties.Author = authorName;

            // Afficher la propriété author
            Console.WriteLine("Document Author: " + workbook.BuiltInDocumentProperties.Author);

            // Enregistrez le classeur
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


