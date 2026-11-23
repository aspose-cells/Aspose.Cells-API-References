---
title: "Font.ArgbColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Font. Obtient et définit la couleur avec une valeur ARGB 32 bits"
type: docs
url: /fr/net/aspose.cells/font/argbcolor/
---
## Font.ArgbColor property

Obtient et définit la couleur avec une valeur ARGB 32 bits.

```csharp
public int ArgbColor { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyArgbColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder aux cellules et définir des valeurs avec différentes couleurs de police
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue("Red Text");
            Style style1 = cell1.GetStyle();
            style1.Font.ArgbColor = unchecked((int)0xFFFF0000); // Red
            cell1.SetStyle(style1);

            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Blue Text");
            Style style2 = cell2.GetStyle();
            style2.Font.ArgbColor = unchecked((int)0xFF0000FF); // Blue
            cell2.SetStyle(style2);

            Cell cell3 = worksheet.Cells["A3"];
            cell3.PutValue("Green Text");
            Style style3 = cell3.GetStyle();
            style3.Font.ArgbColor = unchecked((int)0xFF00FF00); // Green
            cell3.SetStyle(style3);

            // Vérifier et afficher les couleurs
            Console.WriteLine("Cell A1 Font Color: 0x{0:X8}", worksheet.Cells["A1"].GetStyle().Font.ArgbColor);
            Console.WriteLine("Cell A2 Font Color: 0x{0:X8}", worksheet.Cells["A2"].GetStyle().Font.ArgbColor);
            Console.WriteLine("Cell A3 Font Color: 0x{0:X8}", worksheet.Cells["A3"].GetStyle().Font.ArgbColor);
        }
    }
}
```

### Voir aussi

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


