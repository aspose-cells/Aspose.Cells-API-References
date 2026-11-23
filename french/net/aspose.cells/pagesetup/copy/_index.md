---
title: "PageSetup.Copy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode PageSetup. Copie les paramètres de la configuration de la page"
type: docs
url: /fr/net/aspose.cells/pagesetup/copy/
---
## PageSetup.Copy method

Copie les paramètres de la mise en page.

```csharp
public void Copy(PageSetup source, CopyOptions copyOptions)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| source | PageSetup | La source. |
| copyOptions | CopyOptions | Les options de copie. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodCopyWithPageSetupCopyOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // Définissez les propriétés PageSetup pour la première feuille de calcul
            workbook.Worksheets[0].PageSetup.PaperSize = PaperSizeType.PaperA3;
            
            // Copiez PageSetup de la première feuille de calcul vers la deuxième feuille de calcul avec CopyOptions
            workbook.Worksheets[1].PageSetup.Copy(workbook.Worksheets[0].PageSetup, new CopyOptions());
            
            Console.WriteLine("Paper size of second worksheet: " + workbook.Worksheets[1].PageSetup.PaperSize);
        }
    }
}
```

### Voir aussi

* class [CopyOptions](../../copyoptions/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


