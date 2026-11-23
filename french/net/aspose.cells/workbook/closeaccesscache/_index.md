---
title: "Workbook.CloseAccessCache"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Ferme la session qui utilise des caches pour accéder aux données"
type: docs
url: /fr/net/aspose.cells/workbook/closeaccesscache/
---
## Workbook.CloseAccessCache method

Ferme la session qui utilise des caches pour accéder aux données.

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
    public class WorkbookMethodCloseAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ajoutez des données d'exemple et un formatage conditionnel
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue(i % 2 == 0 ? "Data" : "Other");
            }

            // Ajouter une mise en forme conditionnelle
            int ruleIdx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[ruleIdx];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Equal, "Data", null);
            Style style = workbook.CreateStyle();
            style.Font.Size = 16;
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 9, EndColumn = 0 });
            fcc[0].Style = style;

            // Démarrer le cache d'accès pour le formatage conditionnel
            workbook.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Accéder aux cellules avec le formatage conditionnel mis en cache
            for (int i = 0; i < 10; i++)
            {
                Cell cell = cells[i, 0];
                Console.WriteLine($"Cell {cell.Name}: Value={cell.StringValue}, FontSize={cell.GetDisplayStyle().Font.Size}");
            }

            // Fermer le cache d'accès
            workbook.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


