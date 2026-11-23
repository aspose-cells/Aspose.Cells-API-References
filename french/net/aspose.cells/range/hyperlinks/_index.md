---
title: "Range.Hyperlinks"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Range. Obtient tous les hyperliens dans la plage"
type: docs
url: /fr/net/aspose.cells/range/hyperlinks/
---
## Range.Hyperlinks property

Obtient tous les hyperliens dans la plage.

```csharp
public Hyperlink[] Hyperlinks { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyHyperlinksDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter un lien hypertexte à la cellule A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // Créez une plage contenant A1
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1");
            
            // Obtenez les hyperliens dans la plage
            Hyperlink[] hyperlinks = range.Hyperlinks;
            
            // Affichez les informations sur les hyperliens
            if (hyperlinks.Length > 0)
            {
                Console.WriteLine("Hyperlink found:");
                Console.WriteLine($"Address: {hyperlinks[0].Address}");
                Console.WriteLine($"Link Type: {hyperlinks[0].LinkType}");
                
                // Supprimer l'hyperlien
                hyperlinks[0].Delete();
                Console.WriteLine("Hyperlink deleted");
            }
            
            // Vérifier que le lien hypertexte a été supprimé
            Console.WriteLine($"Total hyperlinks in worksheet: {worksheet.Hyperlinks.Count}");
        }
    }
}
```

### Voir aussi

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


