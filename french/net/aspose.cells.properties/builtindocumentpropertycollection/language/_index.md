---
title: "BuiltInDocumentPropertyCollection.Language"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BuiltInDocumentPropertyCollection. Obtient ou définit la langue du document"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/language/
---
## BuiltInDocumentPropertyCollection.Language property

Obtient ou définit la langue du document.

```csharp
public string Language { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLanguageDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accédez à la collection intégrée des propriétés du document
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Définir la propriété language
            builtInProperties.Language = "en-US";

            // Définir d'autres propriétés de base pour la démonstration
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Language Property Demo";

            // Enregistrez le classeur
            workbook.Save("LanguagePropertyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


