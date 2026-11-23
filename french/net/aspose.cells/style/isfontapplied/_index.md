---
title: "Style.IsFontApplied"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Indique si le formatage de police doit être appliqué"
type: docs
url: /fr/net/aspose.cells/style/isfontapplied/
---
## Style.IsFontApplied property

Indique si le formatage de police doit être appliqué.

```csharp
public bool IsFontApplied { get; set; }
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
    public class StylePropertyIsFontAppliedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accédez à une cellule de la feuille de calcul
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            
            // Obtenir le style de la cellule
            Style style = cell.GetStyle();
            
            // Appliquer les paramètres de police
            style.Font.Name = "Times New Roman";
            style.Font.Size = 14;
            style.Font.Color = Color.Blue;
            
            // Activer l'application de la police
            style.IsFontApplied = true;
            
            // Appliquer le style modifié à la cellule
            cell.SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("FontAppliedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


