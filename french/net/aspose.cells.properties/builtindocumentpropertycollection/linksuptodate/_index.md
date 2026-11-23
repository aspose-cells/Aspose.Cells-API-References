---
title: "BuiltInDocumentPropertyCollection.LinksUpToDate"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "BuiltInDocumentPropertyCollection property. Indique si les hyperliens dans un document sont à jour"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/linksuptodate/
---
## BuiltInDocumentPropertyCollection.LinksUpToDate property

Indique si les hyperliens dans un document sont à jour.

```csharp
public bool LinksUpToDate { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLinksUpToDateDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accédez à la collection intégrée des propriétés du document
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Définir la propriété LinksUpToDate pour indiquer si les hyperliens sont actuels
            builtInProperties.LinksUpToDate = true;

            // Ajouter un hyperlien simple pour démontrer la propriété
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Enregistrez le classeur
            workbook.Save("LinksUpToDateDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


