---
title: "Protection.AllowInsertingHyperlink"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Protection property. Représente si l'insertion d'hyperliens est autorisée sur une feuille de calcul protégée"
type: docs
url: /fr/net/aspose.cells/protection/allowinsertinghyperlink/
---
## Protection.AllowInsertingHyperlink property

Représente si l'insertion d'hyperliens est autorisée sur une feuille de calcul protégée

```csharp
public bool AllowInsertingHyperlink { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingHyperlinkDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Protection protection = worksheet.Protection;
            protection.AllowInsertingHyperlink = true;
            protection.Password = "password123";

            // Ajouter un hyperlien pour démontrer la fonctionnalité
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            workbook.Save("AllowInsertingHyperlinkDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


