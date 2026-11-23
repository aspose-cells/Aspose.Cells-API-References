---
title: "Cell.GetPrecedents"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Obtient toutes les références apparaissant dans la formule de cette cellule"
type: docs
url: /fr/net/aspose.cells/cell/getprecedents/
---
## Cell.GetPrecedents method

Obtient toutes les références apparaissant dans la formule de cette cellule.

```csharp
public ReferredAreaCollection GetPrecedents()
```

### Valeur de retour

Collection de toutes les références apparaissant dans la formule de cette cellule.

### Remarques

Renvoie null si ce n'est pas une cellule de formule. Toutes les références apparaissant dans la formule de cette cellule seront renvoyées, qu'elles soient référencées ou non lors du calcul. Par exemple, bien que la cellule A2 dans la formule "=IF(TRUE,A1,A2)" ne soit pas utilisée lors du calcul, elle est toujours considérée comme un antécédent de la formule. Pour obtenir uniquement les références qui influencent le calcul, veuillez utiliser [`GetPrecedentsInCalculation`](../getprecedentsincalculation/).

### Exemples

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetPrecedentsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Définir la formule avec les antécédents
            cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1";
            
            // Obtenir toutes les références d'antécédents
            ReferredAreaCollection areas = cells["A1"].GetPrecedents();
            
            // Afficher chaque référence d'antécédent
            foreach (ReferredArea area in areas)
            {
                StringBuilder sb = new StringBuilder();
                if (area.IsExternalLink)
                {
                    sb.Append($"[{area.ExternalFileName}]");
                }
                sb.Append($"{area.SheetName}!");
                sb.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
                if (area.IsArea)
                {
                    sb.Append($":{CellsHelper.CellIndexToName(area.EndRow, area.EndColumn)}");
                }
                Console.WriteLine(sb.ToString());
            }
        }
    }
}
```

### Voir aussi

* class [ReferredAreaCollection](../../referredareacollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


