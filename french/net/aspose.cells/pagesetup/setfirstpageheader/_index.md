---
title: "PageSetup.SetFirstPageHeader"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PageSetup. Définit un script formatant l'en-tête de première page d'un fichier Excel. N'a d'effet que dans Excel 2007 lorsque IsHFDiffFirst est vrai"
type: docs
url: /fr/net/aspose.cells/pagesetup/setfirstpageheader/
---
## PageSetup.SetFirstPageHeader method

Définit un script formatant l'en-tête de la première page d'un fichier Excel. N'a d'effet que dans Excel 2007 lorsque IsHFDiffFirst est vrai.

```csharp
public void SetFirstPageHeader(int section, string headerScript)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| section | Int32 | 0 : Section gauche, 1 : Section centrale, 2 : Section droite. |
| headerScript | String | Script de format d’en-tête. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFirstPageHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Définir l'en-tête de première page avec le numéro de section et le texte d'en-tête
            pageSetup.SetFirstPageHeader(2, "&CHeader Text");

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


