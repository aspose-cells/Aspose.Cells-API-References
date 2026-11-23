---
title: "WorksheetCollection.ExternalLinks"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorksheetCollection. Représente les liens externes dans un classeur"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/externallinks/
---
## WorksheetCollection.ExternalLinks property

Représente les liens externes dans un classeur.

```csharp
public ExternalLinkCollection ExternalLinks { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyExternalLinksDemo
    {
        public static void Run()
        {
            // Créer un classeur source avec un lien externe
            var sourceWorkbook = new Workbook();
            sourceWorkbook.Worksheets.Add("Sheet1");
            sourceWorkbook.Worksheets.ExternalLinks.Add("external.xlsx", new string[] { "Sheet1!A1" });
            
            // Créer un classeur de destination
            var destWorkbook = new Workbook();
            destWorkbook.Worksheets.Add("Sheet1");

            // Définir la source de données du lien externe
            Console.WriteLine("Original external link: {0}", sourceWorkbook.Worksheets.ExternalLinks[0].DataSource);
            sourceWorkbook.Worksheets.ExternalLinks[0].DataSource = "updated_external.xlsx";
            Console.WriteLine("Updated external link: {0}", sourceWorkbook.Worksheets.ExternalLinks[0].DataSource);

            // Enregistrez le classeur
            sourceWorkbook.Save("output.xlsx");
            Console.WriteLine("Workbook saved with updated external link.");

            // Nettoyer
            sourceWorkbook.Dispose();
            destWorkbook.Dispose();
        }
    }
}
```

### Voir aussi

* class [ExternalLinkCollection](../../externallinkcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


