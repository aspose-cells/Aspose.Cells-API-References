---
title: "PageSetup.SetEvenHeader"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PageSetup. Définit un script formatant l'en-tête de page paire d'un fichier Excel. N'a d'effet que dans Excel 2007 lorsque IsHFDiffOddEven est vrai"
type: docs
url: /fr/net/aspose.cells/pagesetup/setevenheader/
---
## PageSetup.SetEvenHeader method

Définit un script formatant l'en-tête pair d'un fichier Excel. N'a d'effet que dans Excel 2007 lorsque IsHFDiffOddEven est vrai.

```csharp
public void SetEvenHeader(int section, string headerScript)
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
    public class PageSetupMethodSetEvenHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Activer des en-têtes/pieds de page différents pour les pages impaires et paires
            pageSetup.IsHFDiffOddEven = true;

            // Définir l'en-tête de page paire avec l'index de section et le texte
            pageSetup.SetEvenHeader(1, "Even Page Header - Center Section");
            pageSetup.SetEvenHeader(0, "Even Page Header - Left Section");
            pageSetup.SetEvenHeader(2, "Even Page Header - Right Section");

            // Enregistrez le classeur
            workbook.Save("PageSetup_SetEvenHeaderExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


