---
title: "Font.IsItalic"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Font. Obtient ou définit une valeur indiquant si la police est en italique"
type: docs
url: /fr/net/aspose.cells/font/isitalic/
---
## Font.IsItalic property

Obtient ou définit une valeur indiquant si la police est en italique.

```csharp
public bool IsItalic { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsItalicDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accédez au style par défaut
            Style style = workbook.DefaultStyle;
            
            // Définissez les propriétés de la police incluant IsItalic
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.Font.IsItalic = true;
            
            // Appliquer le style à la cellule A1
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Italic Text Example");
            
            // Enregistrez le classeur
            workbook.Save("FontPropertyIsItalicDemo.xlsx");
            
            // Vérifiez la propriété italique
            Console.WriteLine("Font is italic: " + cell.GetStyle().Font.IsItalic);
        }
    }
}
```

### Voir aussi

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


