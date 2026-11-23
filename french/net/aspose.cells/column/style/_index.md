---
title: "Column.Style"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Column. Obtient le style de cette colonne"
type: docs
url: /fr/net/aspose.cells/column/style/
---
## Column.Style property

Obtient le style de cette colonne.

```csharp
[Obsolete("Use Column.GetStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style Style { get; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Column.GetStyle() pour obtenir le style par défaut de cette colonne. Cette propriété sera supprimée 12 mois plus tard, depuis décembre 2022. Aspose s'excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnPropertyStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Accéder à la première colonne
            Column column = worksheet.Cells.Columns[0];
            
            // Obtenir le style actuel en utilisant la propriété Style
            Style originalStyle = column.Style;
            Console.WriteLine("Original column style - Background: " + originalStyle.BackgroundColor);
            
            // Créer un nouveau style et modifier les propriétés
            Style newStyle = workbook.CreateStyle();
            newStyle.BackgroundColor = Color.LightBlue;
            newStyle.Font.IsBold = true;
            newStyle.HorizontalAlignment = TextAlignmentType.Center;
            
            // Appliquer le nouveau style à la colonne
            column.SetStyle(newStyle);
            
            // Ajouter des données pour démontrer l'application du style
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            
            // Vérifier les changements de style
            Console.WriteLine("New column style applied - Background: " + column.GetStyle().BackgroundColor);
            
            // Enregistrer avec ajustement de la largeur de colonne
            column.Width = 15;
            workbook.Save("ColumnStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


