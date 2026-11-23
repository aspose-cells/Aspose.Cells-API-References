---
title: "Hyperlink.LinkType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Hyperlink. Obtient le type de lien"
type: docs
url: /fr/net/aspose.cells/hyperlink/linktype/
---
## Hyperlink.LinkType property

Obtient le type de lien.

```csharp
public TargetModeType LinkType { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyLinkTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un hyperlien externe
            int hyperlinkIndex = worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            Hyperlink link = worksheet.Hyperlinks[hyperlinkIndex];
            
            // Démontrez la propriété LinkType
            Console.WriteLine("Hyperlink LinkType: " + link.LinkType);
            
            // Nettoyer
            link.Delete();
            Console.WriteLine("Hyperlinks count after deletion: " + worksheet.Hyperlinks.Count);
        }
    }
}
```

### Voir aussi

* enum [TargetModeType](../../targetmodetype/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


