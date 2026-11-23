---
title: "Style.IsFillApplied"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Indique si le format de remplissage doit être appliqué"
type: docs
url: /fr/net/aspose.cells/style/isfillapplied/
---
## Style.IsFillApplied property

Indique si le formatage de remplissage doit être appliqué.

```csharp
public bool IsFillApplied { get; set; }
```

### Remarques

Uniquement pour le style nommé.

### Exemples

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyIsFillAppliedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer un style
            Style style = workbook.CreateStyle();
            
            // Initialement, IsFillApplied doit être false
            Console.WriteLine("IsFillApplied (initial): " + style.IsFillApplied);
            
            // Appliquer les paramètres de remplissage
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Après avoir défini les propriétés de remplissage, IsFillApplied doit être true
            Console.WriteLine("IsFillApplied (after setting fill): " + style.IsFillApplied);
            
            // Appliquer le style à une cellule
            worksheet.Cells["A1"].SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("IsFillAppliedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


