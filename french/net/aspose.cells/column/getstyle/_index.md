---
title: "Column.GetStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Column. Obtient le style de cette colonne"
type: docs
url: /fr/net/aspose.cells/column/getstyle/
---
## Column.GetStyle method

Obtient le style de cette colonne.

```csharp
public Style GetStyle()
```

### Remarques

La modification directe de l'objet style retourné n'a aucun effet sur cette colonne ou sur les cellules de cette colonne. Vous devez appeler la méthode [`ApplyStyle`](../applystyle/) ou [`SetStyle`](../setstyle/) pour appliquer le changement à cette colonne. Le style de la colonne est le style qui sera hérité par les cellules de cette colonne (ces cellules qui n'ont pas de paramètres de style personnalisés, comme les cellules existantes qui n'ont pas eu de style défini explicitement, ou celles qui n'ont pas été instanciées).

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnMethodGetStyleDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir le style pour la colonne 5
            Style columnStyle = cells.Columns[5].GetStyle();
            columnStyle.Font.Name = "Arial";
            columnStyle.Font.Size = 14;
            columnStyle.Font.IsBold = true;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { Font = true });

            // Définir le style pour la ligne 7
            Style rowStyle = cells.Rows[7].GetStyle();
            rowStyle.Font.Color = System.Drawing.Color.Red;
            rowStyle.Font.IsItalic = true;
            cells.Rows[7].ApplyStyle(rowStyle, new StyleFlag { Font = true });

            // Vérifiez le style de la colonne
            Style retrievedColumnStyle = cells.Columns[5].GetStyle();
            Console.WriteLine("Column 5 Style:");
            Console.WriteLine($"Font: {retrievedColumnStyle.Font.Name}, Size: {retrievedColumnStyle.Font.Size}, Bold: {retrievedColumnStyle.Font.IsBold}");

            // Vérifiez le style de la ligne
            Style retrievedRowStyle = cells.Rows[7].GetStyle();
            Console.WriteLine("\nRow 7 Style:");
            Console.WriteLine($"Color: {retrievedRowStyle.Font.Color}, Italic: {retrievedRowStyle.Font.IsItalic}");

            // Enregistrez le classeur
            workbook.Save("ColumnMethodGetStyleDemo_output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


