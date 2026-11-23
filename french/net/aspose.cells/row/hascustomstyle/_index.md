---
title: "Row.HasCustomStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Row. Indique si cette ligne possède des paramètres de style personnalisés différents du style par défaut hérité du classeur"
type: docs
url: /fr/net/aspose.cells/row/hascustomstyle/
---
## Row.HasCustomStyle property

Indique si cette ligne possède des paramètres de style personnalisés(différents de ceux par défaut hérités du classeur).

```csharp
public bool HasCustomStyle { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer et personnaliser un style
            Style customStyle = workbook.CreateStyle();
            customStyle.BackgroundColor = Color.LightBlue;
            customStyle.Pattern = BackgroundType.Solid;
            
            // Accéder à la première ligne
            Row row = worksheet.Cells.Rows[0];
            
            // Appliquer un style personnalisé à la ligne
            row.ApplyStyle(customStyle, new StyleFlag { All = true });
            
            // Vérifier si la ligne a un style personnalisé (devrait être vrai)
            bool hasCustomStyle = row.HasCustomStyle;
            Console.WriteLine("Row has custom style: " + hasCustomStyle);
            
            // Enregistrez le classeur
            workbook.Save("RowHasCustomStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


