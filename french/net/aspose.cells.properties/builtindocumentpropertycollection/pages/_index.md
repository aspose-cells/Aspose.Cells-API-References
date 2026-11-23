---
title: "BuiltInDocumentPropertyCollection.Pages"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BuiltInDocumentPropertyCollection. Représente une estimation du nombre de pages dans le document"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/pages/
---
## BuiltInDocumentPropertyCollection.Pages property

Représente une estimation du nombre de pages dans le document.

```csharp
public int Pages { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyPagesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux propriétés de document intégrées
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Définissez la propriété Pages
            builtInProperties.Pages = 10;

            // Ajouter une feuille de calcul et des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Page Count Demonstration");
            worksheet.Cells["A2"].PutValue($"This document is set to have {builtInProperties.Pages} pages");

            // Enregistrez le classeur
            workbook.Save("DocumentPagesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


