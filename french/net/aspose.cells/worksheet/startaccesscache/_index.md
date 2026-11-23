---
title: "Worksheet.StartAccessCache"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Worksheet. Démarre la session qui utilise des caches pour accéder aux données de cette feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/startaccesscache/
---
## Worksheet.StartAccessCache method

Démarre la session qui utilise des caches pour accéder aux données de cette feuille de calcul.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| opts | AccessCacheOptions | options d'accès aux données |

### Remarques

Après avoir terminé l'accès aux données, [`CloseAccessCache`](../closeaccesscache/) doit être invoqué avec les mêmes options pour vider tous les caches et rétablir le mode d'accès normal.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodStartAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Définir le style par défaut
            Style style = wb.DefaultStyle;
            style.Font.Size = 10;
            wb.DefaultStyle = style;

            // Ajouter une mise en forme conditionnelle
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 10, 10));
            fcc.AddCondition(FormatConditionType.DuplicateValues);
            FormatCondition fc = fcc[0];
            fc.Style.Font.Size = 16;

            // Remplissez quelques données
            Cells cells = sheet.Cells;
            for (int i = 0; i < 10; i++)
            {
                cells[0, i].PutValue("A");
                cells[i, 0].PutValue(i);
            }

            // Démarrer le cache d'accès pour de meilleures performances
            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Vérifier les styles
            for (int i = 0; i < 10; i++)
            {
                Console.WriteLine($"Cell[0,{i}] Font Size: {cells[0, i].GetDisplayStyle().Font.Size}");
                Console.WriteLine($"Cell[{i},0] Font Size: {cells[i, 0].GetDisplayStyle().Font.Size}");
            }

            // Fermer le cache une fois terminé
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


