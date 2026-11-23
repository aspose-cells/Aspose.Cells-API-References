---
title: "Hyperlink.ScreenTip"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Hyperlink. Retourne ou définit le texte ScreenTip pour le lien hypertexte spécifié."
type: docs
url: /fr/net/aspose.cells/hyperlink/screentip/
---
## Hyperlink.ScreenTip property

Renvoie ou définit le texte ScreenTip pour le lien hypertexte spécifié.

```csharp
public string ScreenTip { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkPropertyScreenTipDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Click this hyperlink:");

            // Créez un lien hypertexte avec ScreenTip
            int hLinkIdx = worksheet.Hyperlinks.Add("B1", 1, 1, "https://www.aspose.com");
            worksheet.Hyperlinks[hLinkIdx].ScreenTip = "Visit Aspose website for more information";

            // Enregistrez le classeur
            workbook.Save("HyperlinkWithScreenTip.xlsx");
        }
    }
}
```

### Voir aussi

* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


