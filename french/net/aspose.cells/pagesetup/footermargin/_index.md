---
title: "PageSetup.FooterMargin"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente la distance entre le bas de la page et le pied de page en centimètres"
type: docs
url: /fr/net/aspose.cells/pagesetup/footermargin/
---
## PageSetup.FooterMargin property

Représente la distance entre le bas de la page et le pied de page, en centimètres.

```csharp
public double FooterMargin { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFooterMarginDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Accédez à PageSetup
            PageSetup pageSetup = worksheet.PageSetup;

            // Définir la marge du pied de page en centimètres
            pageSetup.FooterMargin = 1.5;

            // Ajoutez du contenu pour voir l'effet
            worksheet.Cells["A1"].PutValue("Footer Margin Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates setting footer margin to 1.5 cm");

            // Définir le texte du pied de page pour rendre la marge visible
            pageSetup.SetFooter(0, "&A - Footer text to demonstrate margin");

            // Enregistrez le classeur
            workbook.Save("FooterMarginDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


