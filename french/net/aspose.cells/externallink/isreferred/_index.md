---
title: "ExternalLink.IsReferred"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalLink. Indique si ce lien externe est référencé par d'autres"
type: docs
url: /fr/net/aspose.cells/externallink/isreferred/
---
## ExternalLink.IsReferred property

Indique si ce lien externe est référencé par d’autres.

```csharp
public bool IsReferred { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyIsReferredDemo
    {
        public static void Run()
        {
            // Créer un classeur avec un lien externe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter une référence de lien externe
            worksheet.Cells["A1"].Formula = "='[external.xlsx]Sheet1'!A1";
            
            // Vérifier si le lien externe est référencé
            if (workbook.Worksheets.ExternalLinks.Count > 0)
            {
                bool isReferred = workbook.Worksheets.ExternalLinks[0].IsReferred;
                Console.WriteLine("Is external link referred: " + isReferred);
            }
        }
    }
}
```

### Voir aussi

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


