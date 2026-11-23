---
title: "Style.BackgroundColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Obtient ou définit la couleur d’arrière-plan d’un style"
type: docs
url: /fr/net/aspose.cells/style/backgroundcolor/
---
## Style.BackgroundColor property

Obtient ou définit la couleur d'arrière-plan d'un style.

```csharp
public Color BackgroundColor { get; set; }
```

### Remarques

Si vous souhaitez définir la couleur d’une cellule, veuillez utiliser la propriété Style.ForegroundColor. Cette propriété ne prendra effet que si le modèle de style de la cellule est différent de « none » ou « solid ».

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créez un objet de style
            Style style = workbook.CreateStyle();
            
            // Définissez la couleur d’arrière-plan sur jaune
            style.BackgroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Appliquer le style à la cellule A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Cell with yellow background");
            cell.SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


