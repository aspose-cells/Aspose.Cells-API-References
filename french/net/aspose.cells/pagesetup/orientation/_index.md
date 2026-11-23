---
title: "PageSetup.Orientation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PageSetup. Représente l'orientation d'impression de la page"
type: docs
url: /fr/net/aspose.cells/pagesetup/orientation/
---
## PageSetup.Orientation property

Représente l'orientation d'impression de la page.

```csharp
public PageOrientationType Orientation { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyOrientationDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définissez l'orientation de la page sur Landscape
            worksheet.PageSetup.Orientation = PageOrientationType.Landscape;
            
            // Ajoutez des données d'exemple pour démontrer l'effet
            worksheet.Cells["A1"].PutValue("Landscape Orientation Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue($"Data Row {i}");
            }
            
            // Enregistrez le classeur
            workbook.Save("PageOrientationDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* enum [PageOrientationType](../../pageorientationtype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


