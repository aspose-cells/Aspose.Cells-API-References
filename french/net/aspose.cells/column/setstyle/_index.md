---
title: "Column.SetStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Column. Définit le style de cette colonne"
type: docs
url: /fr/net/aspose.cells/column/setstyle/
---
## Column.SetStyle method

Définit le style de cette colonne.

```csharp
public void SetStyle(Style style)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| style | Style | le style à utiliser comme style par défaut pour les cellules de cette colonne. |

### Remarques

Cette méthode ne définit le style donné que comme style par défaut pour cette colonne, sans modifier les paramètres de style des cellules existantes dans cette colonne. Pour mettre à jour les paramètres de style des cellules existantes vers le style spécifié en même temps, veuillez utiliser [`ApplyStyle`](../applystyle/)

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnMethodSetStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la première colonne
            Column column = worksheet.Cells.Columns[0];

            // Créer un nouveau style à partir du classeur
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.LightBlue;
            style.Pattern = BackgroundType.Solid;

            try
            {
                // Appliquer le style personnalisé à toute la colonne
                column.SetStyle(style);
                
                Console.WriteLine($"Style applied successfully to column {column.Index}");
                Console.WriteLine($"Font: {style.Font.Name}, Size: {style.Font.Size}, Bold: {style.Font.IsBold}");
                Console.WriteLine($"Background: {style.ForegroundColor.Name}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStyle method: {ex.Message}");
            }

            // Enregistrer le classeur modifié
            workbook.Save("ColumnMethodSetStyleDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


