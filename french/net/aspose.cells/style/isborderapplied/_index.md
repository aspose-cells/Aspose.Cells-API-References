---
title: "Style.IsBorderApplied"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Style. Indique si le formatage des bordures doit être appliqué"
type: docs
url: /fr/net/aspose.cells/style/isborderapplied/
---
## Style.IsBorderApplied property

Indique si le formatage des bordures doit être appliqué.

```csharp
public bool IsBorderApplied { get; set; }
```

### Remarques

Uniquement pour le style nommé.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyIsBorderAppliedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer un style personnalisé
            Style style = workbook.CreateStyle();
            
            // Appliquer les paramètres de bordure au style
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Black;
            
            // Vérifier si la bordure est appliquée
            Console.WriteLine("IsBorderApplied before setting: " + style.IsBorderApplied);
            
            // Définissez explicitement IsBorderApplied sur true
            style.IsBorderApplied = true;
            
            // Appliquer le style à une cellule
            worksheet.Cells["A1"].SetStyle(style);
            
            // Vérifier l'application des bordures
            Console.WriteLine("IsBorderApplied after setting: " + style.IsBorderApplied);
            
            // Enregistrez le classeur
            workbook.Save("IsBorderAppliedDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


