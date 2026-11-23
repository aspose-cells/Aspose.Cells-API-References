---
title: "Font.Name"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Font. Obtient ou définit le nom de la police"
type: docs
url: /fr/net/aspose.cells/font/name/
---
## Font.Name property

Obtient ou définit le nom du [`Font`](../).

```csharp
public virtual string Name { get; set; }
```

### Remarques

Si cette propriété est utilisée pour définir le nom de la police, le [`SchemeType`](../schemetype/) sera mis à jour à None

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyNameDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la feuille de calcul et aux cellules par défaut
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Créer et modifier un style avec des propriétés de police
            Style style = workbook.CreateStyle();
            Font font = style.Font;
            
            // Démontrer l'utilisation de la propriété Name
            font.Name = "Arial";  // Changed from FontNameConstants.Arial to string literal
            font.Size = 14;
            font.IsBold = true;
            
            // Appliquer le style à une cellule
            cells["A1"].PutValue("Font Property Name Demo");
            cells["A1"].SetStyle(style);
            
            // Enregistrez le classeur
            workbook.Save("FontPropertyNameDemo.xlsx");
            
            Console.WriteLine("Demo completed. File saved as FontPropertyNameDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


