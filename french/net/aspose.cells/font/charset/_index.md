---
title: "Font.Charset"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Font. Représente le jeu de caractères"
type: docs
url: /fr/net/aspose.cells/font/charset/
---
## Font.Charset property

Représente le jeu de caractères.

```csharp
public int Charset { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyCharsetDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer un style avec des propriétés de police spécifiques, y compris le jeu de caractères
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.Charset = 1; // ANSI_CHARSET

            // Appliquer le style à une cellule
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Text with ANSI charset");

            // Créer un autre style avec un jeu de caractères différent
            Style style2 = workbook.CreateStyle();
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 12;
            style2.Font.Charset = 2; // DEFAULT_CHARSET

            // Appliquer le deuxième style à une autre cellule
            Cell cell2 = worksheet.Cells["A2"];
            cell2.SetStyle(style2);
            cell2.PutValue("Text with DEFAULT charset");

            // Enregistrez le classeur
            workbook.Save("FontCharsetDemo.xlsx");

            // Vérifier les propriétés du jeu de caractères
            Console.WriteLine("Cell A1 Font Charset: " + cell.GetStyle().Font.Charset);
            Console.WriteLine("Cell A2 Font Charset: " + cell2.GetStyle().Font.Charset);
        }
    }
}
```

### Voir aussi

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


