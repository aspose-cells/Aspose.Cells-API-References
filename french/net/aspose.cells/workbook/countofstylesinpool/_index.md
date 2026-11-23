---
title: "Workbook.CountOfStylesInPool"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Obtient le nombre de styles dans le pool de styles"
type: docs
url: /fr/net/aspose.cells/workbook/countofstylesinpool/
---
## Workbook.CountOfStylesInPool property

Obtient le nombre de styles dans le pool de styles.

```csharp
public int CountOfStylesInPool { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCountOfStylesInPoolDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook wb = new Workbook();
            
            // Obtenir le nombre initial de styles dans le pool
            int initialStyleCount = wb.CountOfStylesInPool;
            Console.WriteLine($"Initial styles in pool: {initialStyleCount}");

            // Ajouter quelques styles en modifiant les cellules
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Style 1
            Style style1 = wb.CreateStyle();
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            cells["A1"].SetStyle(style1);
            
            // Style 2
            Style style2 = wb.CreateStyle();
            style2.Font.Color = System.Drawing.Color.Red;
            style2.Pattern = BackgroundType.Solid;
            cells["B1"].SetStyle(style2);

            // Obtenir le nombre de styles mis à jour
            int updatedStyleCount = wb.CountOfStylesInPool;
            Console.WriteLine($"Styles after modifications: {updatedStyleCount}");

            // Enregistrer pour démontrer la persistance des styles
            wb.Save("output.html", SaveFormat.Html);
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


