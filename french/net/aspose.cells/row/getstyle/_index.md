---
title: "Row.GetStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Row. Obtient le style de cette ligne"
type: docs
url: /fr/net/aspose.cells/row/getstyle/
---
## Row.GetStyle method

Obtient le style de cette ligne.

```csharp
public Style GetStyle()
```

### Remarques

Modifier directement l'objet style retourné n'a aucun effet sur cette ligne ou sur les cellules de cette ligne. Vous devez appeler la méthode [`ApplyStyle`](../applystyle/) ou [`SetStyle`](../setstyle/) pour appliquer la modification à cette ligne. Le style de la ligne est le style qui sera hérité par les cellules de cette ligne (ces cellules qui n'ont pas de paramètres de style personnalisés, comme les cellules existantes dont le style n'a pas été défini explicitement, ou celles qui n'ont pas été instanciées).

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetStyleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Définir les styles pour la démonstration
            Style rowStyle = workbook.CreateStyle();
            rowStyle.Pattern = BackgroundType.Solid;
            rowStyle.ForegroundColor = System.Drawing.Color.Blue;
            cells.Rows[8].ApplyStyle(rowStyle, new StyleFlag { All = true });

            Style columnStyle = workbook.CreateStyle();
            columnStyle.Pattern = BackgroundType.Solid;
            columnStyle.ForegroundColor = System.Drawing.Color.Red;
            cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { All = true });

            // Démontrer l'utilisation de GetStyle
            Style retrievedRowStyle = cells.Rows[8].GetStyle();
            Console.WriteLine("Row 8 Style - ForegroundColor: " + retrievedRowStyle.ForegroundColor);
            Console.WriteLine("Row 8 Style - Pattern: " + retrievedRowStyle.Pattern);

            Style retrievedColumnStyle = cells.Columns[5].GetStyle();
            Console.WriteLine("Column 5 Style - ForegroundColor: " + retrievedColumnStyle.ForegroundColor);
            Console.WriteLine("Column 5 Style - Pattern: " + retrievedColumnStyle.Pattern);
        }
    }
}
```

### Voir aussi

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


