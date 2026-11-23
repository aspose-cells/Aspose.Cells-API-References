---
title: "ReferredArea.EndRow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ReferredArea property. La ligne de fin de la zone"
type: docs
url: /fr/net/aspose.cells/referredarea/endrow/
---
## ReferredArea.EndRow property

La ligne de fin de la zone.

```csharp
public int EndRow { get; }
```

### Exemples

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyEndRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Définissez la formule avec plusieurs références
            cells["A1"].Formula = "= B1 + SUM(B1:B10) + [Book1.xls]Sheet1!A1";
            
            // Obtenez toutes les zones précédentes
            ReferredAreaCollection areas = cells["A1"].GetPrecedents();
            
            // Traitez chaque référence
            foreach (ReferredArea area in areas)
            {
                StringBuilder sb = new StringBuilder();
                
                if (area.IsExternalLink)
                {
                    sb.Append($"[{area.ExternalFileName}]");
                }
                
                sb.Append($"{area.SheetName}!");
                sb.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
                
                // Démontrez l'utilisation de EndRow pour les références de plage
                if (area.IsArea)
                {
                    sb.Append($":{CellsHelper.CellIndexToName(area.EndRow, area.EndColumn)}");
                }
                
                Console.WriteLine(sb.ToString());
            }
            
            workbook.Save("ReferredAreaExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


