---
title: "Worksheet.Outline"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Obtient le plan de cette feuille de calcul"
type: docs
url: /fr/net/aspose.cells/worksheet/outline/
---
## Worksheet.Outline property

Obtient le contour de cette feuille de calcul.

```csharp
public Outline Outline { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyOutlineDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple et créez des groupes de plan
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[$"A{i + 1}"].Value = $"Item {i + 1}";
                worksheet.Cells[$"B{i + 1}"].Value = (i + 1) * 100;
            }

            // Regrouper les lignes (crée un plan)
            worksheet.Cells.GroupRows(0, 9, false);

            // Accéder aux propriétés du plan
            Outline outline = worksheet.Outline;
            Console.WriteLine($"Outline summary row is below detail: {outline.SummaryRowBelow}");
            Console.WriteLine($"Outline summary column is to right: {outline.SummaryColumnRight}");

            // Modifier les paramètres du plan
            outline.SummaryRowBelow = true;
            outline.SummaryColumnRight = false;

            // Dégroupez les lignes pour démontrer la fonctionnalité du plan
            worksheet.Cells.UngroupRows(0, 9);

            // Enregistrez le classeur
            workbook.Save("WorksheetOutlineDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Outline](../../outline/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


