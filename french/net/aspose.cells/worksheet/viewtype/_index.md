---
title: "Worksheet.ViewType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Worksheet. Obtient et définit le type de vue"
type: docs
url: /fr/net/aspose.cells/worksheet/viewtype/
---
## Worksheet.ViewType property

Obtient et définit le type de vue.

```csharp
public ViewType ViewType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyViewTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définissez le type de vue sur PageLayoutView et activez la règle
            worksheet.ViewType = ViewType.PageLayoutView;
            worksheet.IsRulerVisible = true;
            
            // Ajoutez du contenu d'exemple pour démontrer la vue
            worksheet.Cells["A1"].PutValue("Page Layout View Demo");
            worksheet.Cells["A2"].PutValue("Ruler is visible in this view");
            
            // Enregistrez le classeur
            workbook.Save("WorksheetViewTypeDemo.xlsx");
            
            Console.WriteLine("Worksheet ViewType demo completed successfully.");
        }
    }
}
```

### Voir aussi

* enum [ViewType](../../viewtype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


