---
title: "Range.ColumnWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Range. Définit ou obtient la largeur de colonne de cette plage"
type: docs
url: /fr/net/aspose.cells/range/columnwidth/
---
## Range.ColumnWidth property

Définit ou obtient la largeur de colonne de cette plage

```csharp
public double ColumnWidth { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangePropertyColumnWidthDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accédez à une plage (colonnes B à D)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B:D");
            
            // Affichez la largeur de colonne actuelle
            Console.WriteLine("Current ColumnWidth: " + range.ColumnWidth);

            // Définissez une nouvelle largeur de colonne (en unités de caractères)
            range.ColumnWidth = 15.0;

            // Remplissez les cellules pour démontrer l'effet
            worksheet.Cells["B1"].PutValue("This is column B");
            worksheet.Cells["C1"].PutValue("This is column C");
            worksheet.Cells["D1"].PutValue("This is column D");

            // Ajuster automatiquement la hauteur des lignes pour afficher le contenu
            worksheet.AutoFitRows();

            // Enregistrez le classeur
            workbook.Save("ColumnWidthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


