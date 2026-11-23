---
title: "PageSetup.CenterVertically"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Indique si la feuille est imprimée centrée verticalement"
type: docs
url: /fr/net/aspose.cells/pagesetup/centervertically/
---
## PageSetup.CenterVertically property

Indique si la feuille est imprimée centrée verticalement.

```csharp
public bool CenterVertically { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyCenterVerticallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accédez à PageSetup et définissez CenterVertically
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.CenterVertically = true;
            
            // Ajoutez des données d'exemple pour visualiser l'effet
            worksheet.Cells["A1"].PutValue("This worksheet content will be centered vertically when printed");
            worksheet.Cells["A2"].PutValue("CenterVertically = true");
            
            // Enregistrez le classeur
            workbook.Save("PageSetup_CenterVertically.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


