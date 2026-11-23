---
title: "ExternalLink.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalLink. Obtient le type du lien externe"
type: docs
url: /fr/net/aspose.cells/externallink/type/
---
## ExternalLink.Type property

Obtient le type du lien externe.

```csharp
public ExternalLinkType Type { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul
            Worksheet sheet = workbook.Worksheets[0];
            
            // Créer un lien externe vers un autre classeur
            sheet.Cells["A1"].Formula = "='[link.xls]Sheet1'!A1";
            
            // Obtenir le lien externe
            ExternalLink externalLink = workbook.Worksheets.ExternalLinks[0];
            
            // Afficher le type de lien externe
            Console.WriteLine("External Link Type: " + externalLink.Type);
            
            // Modifier la source de données du lien externe
            externalLink.DataSource = "d:\\link.xls";
            
            // Enregistrez le classeur
            workbook.Save("ExternalLinkTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ExternalLinkType](../../externallinktype/)
* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


