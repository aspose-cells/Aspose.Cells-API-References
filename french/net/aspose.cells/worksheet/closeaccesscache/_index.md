---
title: "Worksheet.CloseAccessCache"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Ferme la session qui utilise des caches pour accéder aux données de cette feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/closeaccesscache/
---
## Worksheet.CloseAccessCache method

Ferme la session qui utilise des caches pour accéder aux données de cette feuille de calcul.

```csharp
public void CloseAccessCache(AccessCacheOptions opts)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| opts | AccessCacheOptions | options d'accès aux données |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCloseAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Remplir les cellules avec des données d'exemple
            for (int i = 0; i < 1000; i++)
            {
                cells[i, 0].PutValue(i % 10);
            }

            // Ajouter une mise en forme conditionnelle
            FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 999, 0));
            fcs.AddCondition(FormatConditionType.ColorScale);

            // Activer le cache d'accès pour le formatage conditionnel
            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Effectuer des opérations avec un accès mis en cache
            Random random = new Random();
            for (int i = 0; i < 100; i++)
            {
                int r = random.Next(0, 1000);
                var style = cells[r, 0].GetDisplayStyle();
                Console.WriteLine($"Cell ({r},0) style: {style.ForegroundArgbColor:X}");
            }

            // Fermer le cache d'accès
            sheet.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);
        }
    }
}
```

### Voir aussi

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


