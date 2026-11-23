---
title: "Outline.SummaryColumnRight"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Outline. Indique si la colonne de résumé sera positionnée à droite des colonnes de détail dans le plan"
type: docs
url: /fr/net/aspose.cells/outline/summarycolumnright/
---
## Outline.SummaryColumnRight property

Indique si la colonne de synthèse sera positionnée à droite des colonnes de détail dans le plan.

```csharp
public bool SummaryColumnRight { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OutlinePropertySummaryColumnRightDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple et regrouper les lignes
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + (i + 1));
                worksheet.Cells["B" + (i + 1)].PutValue(i * 10);
            }

            // Regrouper les lignes (crée un plan)
            worksheet.Cells.GroupRows(0, 9, false);

            // Obtenir les paramètres du plan
            Outline outline = worksheet.Outline;

            // Définir SummaryColumnRight sur true (les colonnes de résumé apparaîtront à droite des colonnes de détail)
            outline.SummaryColumnRight = true;
            Console.WriteLine("SummaryColumnRight is set to: " + outline.SummaryColumnRight);

            // Enregistrez le classeur
            workbook.Save("OutlinePropertySummaryColumnRightDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


