---
title: "Worksheet.PageSetup"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Représente la description de la configuration de page dans cette feuille"
type: docs
url: /fr/net/aspose.cells/worksheet/pagesetup/
---
## Worksheet.PageSetup property

Représente la description de la mise en page de cette feuille.

```csharp
public PageSetup PageSetup { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPageSetupDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définir les propriétés de mise en page
            worksheet.PageSetup.PrintArea = "A1:L50";
            worksheet.PageSetup.PrintTitleRows = "1:2";
            worksheet.PageSetup.PrintTitleColumns = "A:B";
            worksheet.PageSetup.Orientation = PageOrientationType.Landscape;
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperA4;
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
                worksheet.Cells["B" + (i + 1)].PutValue(i * 100);
            }
            
            // Enregistrez le classeur
            workbook.Save("PageSetupDemo.xlsx");
            
            Console.WriteLine("Worksheet page setup demo completed successfully.");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../../pagesetup/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


