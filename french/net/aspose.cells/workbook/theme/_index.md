---
title: "Workbook.Theme"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Obtient le nom du thème"
type: docs
url: /fr/net/aspose.cells/workbook/theme/
---
## Workbook.Theme property

Obtient le nom du thème.

```csharp
public string Theme { get; }
```

### Exemples

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyThemeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Démontrer la récupération du thème par défaut
            Console.WriteLine("Default theme: " + workbook.Theme);
            
            // Modifier la couleur du thème et vérifier
            workbook.SetThemeColor(ThemeColorType.Accent1, Color.Blue);
            Color accent1 = workbook.GetThemeColor(ThemeColorType.Accent1);
            Console.WriteLine("Modified Accent1 color: " + accent1);
            
            // Enregistrer le classeur pour démontrer la persistance du thème
            workbook.Save("ThemeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


