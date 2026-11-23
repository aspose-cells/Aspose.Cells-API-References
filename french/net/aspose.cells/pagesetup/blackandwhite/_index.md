---
title: "PageSetup.BlackAndWhite"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente si les éléments du document seront imprimés en noir et blanc"
type: docs
url: /fr/net/aspose.cells/pagesetup/blackandwhite/
---
## PageSetup.BlackAndWhite property

Indique si les éléments du document seront imprimés en noir et blanc.

```csharp
public bool BlackAndWhite { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBlackAndWhiteDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtenir l'objet PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Définir la propriété BlackAndWhite sur true
            pageSetup.BlackAndWhite = true;
            Console.WriteLine("BlackAndWhite set to: " + pageSetup.BlackAndWhite);

            // Modifier la propriété BlackAndWhite en false
            pageSetup.BlackAndWhite = false;
            Console.WriteLine("BlackAndWhite changed to: " + pageSetup.BlackAndWhite);

            // Enregistrez le classeur
            workbook.Save("PageSetupBlackAndWhiteDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


