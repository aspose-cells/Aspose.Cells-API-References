---
title: "OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété OdsLoadOptions. Indique si le style par défaut d'Excel est appliqué à l'hyperlien"
type: docs
url: /fr/net/aspose.cells/odsloadoptions/applyexceldefaultstyletohyperlink/
---
## OdsLoadOptions.ApplyExcelDefaultStyleToHyperlink property

Indique si le style par défaut d'Excel est appliqué au lien hypertexte.

```csharp
public bool ApplyExcelDefaultStyleToHyperlink { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsLoadOptionsPropertyApplyExcelDefaultStyleToHyperlinkDemo
    {
        public static void Run()
        {
            // Créez une instance de OdsLoadOptions
            OdsLoadOptions loadOptions = new OdsLoadOptions();

            // Définir la propriété ApplyExcelDefaultStyleToHyperlink
            loadOptions.ApplyExcelDefaultStyleToHyperlink = true;

            // Chargez un fichier ODS avec les options spécifiées
            Workbook workbook = new Workbook("sample.ods", loadOptions);

            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un hyperlien pour démontrer l'application du style
            worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");

            // Enregistrez le classeur dans un nouveau fichier
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [OdsLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


