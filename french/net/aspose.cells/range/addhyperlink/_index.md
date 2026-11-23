---
title: "Range.AddHyperlink"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Range. Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules"
type: docs
url: /fr/net/aspose.cells/range/addhyperlink/
---
## Range.AddHyperlink method

Ajoute un hyperlien à une cellule spécifiée ou à une plage de cellules.

```csharp
public Hyperlink AddHyperlink(string address, string textToDisplay, string screenTip)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| address | String | Adresse de l'hyperlien. |
| textToDisplay | String | Le texte à afficher pour l'hyperlien spécifié. |
| screenTip | String | Le texte screenTip pour le lien hypertexte spécifié. |

### Valeur de retour

[`Hyperlink`](../../hyperlink/) object.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodAddHyperlinkWithStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A1:A5");
            
            // Ajouter un hyperlien avec l'adresse, le texte à afficher et l'infobulle
            range.AddHyperlink("https://www.aspose.com", "Visit Aspose", "Click to go to Aspose website");
            
            // Enregistrez le classeur
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Hyperlink](../../hyperlink/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


