---
title: "PageSetup.HeaderMargin"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente la distance du haut de la page à l'en-tête en centimètres"
type: docs
url: /fr/net/aspose.cells/pagesetup/headermargin/
---
## PageSetup.HeaderMargin property

Représente la distance entre le haut de la page et l'en-tête, en centimètres.

```csharp
public double HeaderMargin { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyHeaderMarginDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Accédez à PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Définir la marge d'en-tête en centimètres
            pageSetup.HeaderMargin = 1.5;

            // Vérifier que la marge d'en-tête a été définie
            Console.WriteLine("Header Margin: " + pageSetup.HeaderMargin + " cm");

            // Enregistrez le classeur
            workbook.Save("HeaderMarginDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


