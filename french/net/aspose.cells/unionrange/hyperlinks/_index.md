---
title: "UnionRange.Hyperlinks"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété UnionRange. Obtient tous les hyperliens dans la plage"
type: docs
url: /fr/net/aspose.cells/unionrange/hyperlinks/
---
## UnionRange.Hyperlinks property

Obtient tous les hyperliens dans la plage.

```csharp
public Hyperlink[] Hyperlinks { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyHyperlinksDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter quelques hyperliens aux cellules
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks.Add("B2", 1, 1, "https://products.aspose.com/cells");
            worksheet.Hyperlinks.Add("C3", 1, 1, "https://docs.aspose.com/cells/net");

            // Créez une plage
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C3");
            UnionRange unionRange = range.UnionRanges(new Aspose.Cells.Range[] { range });

            // Obtenez les hyperliens dans la plage
            Hyperlink[] hyperlinks = unionRange.Hyperlinks;
            Console.WriteLine("Hyperlinks count in range: " + hyperlinks.Length);

            // Afficher des informations sur chaque hyperlien
            foreach (Hyperlink link in hyperlinks)
            {
                Console.WriteLine("Address: " + link.Address + ", Text: " + link.TextToDisplay);
            }

            // Enregistrez le classeur
            workbook.Save("HyperlinksDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Hyperlink](../../hyperlink/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


