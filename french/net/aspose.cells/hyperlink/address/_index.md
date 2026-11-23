---
title: "Hyperlink.Address"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Hyperlink. Représente l'adresse d'un hyperlien"
type: docs
url: /fr/net/aspose.cells/hyperlink/address/
---
## Hyperlink.Address property

Représente l'adresse d'un hyperlien.

```csharp
public string Address { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyAddressDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des hyperliens avec des adresses différentes
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.baidu.com/");
            worksheet.Hyperlinks.Add("B1", 1, 1, "http://www.google.com/");
            worksheet.Hyperlinks.Add("C1", 1, 1, "Sheet1!F3");

            // Accéder et afficher les adresses des hyperliens
            HyperlinkCollection links = worksheet.Hyperlinks;
            Console.WriteLine("Hyperlink Count: " + links.Count);
            Console.WriteLine("Link 1 Address: " + links[0].Address);
            Console.WriteLine("Link 2 Address: " + links[1].Address);
            Console.WriteLine("Link 3 Address: " + links[2].Address);

            // Enregistrez le classeur
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


