---
title: "Classe MsoLineFormatHelper"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.MsoLineFormatHelper class. Représente le format des lignes et des pointes de flèche"
type: docs
url: /fr/net/aspose.cells.drawing/msolineformathelper/
---
## MsoLineFormatHelper class

Représente le format des lignes et des pointes de flèche.

```csharp
public class MsoLineFormatHelper
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msolineformathelper/backcolor/) { get; set; } | Obtient et définit la couleur d'arrière-plan de la ligne de bordure. |
| [DashStyle](../../aspose.cells.drawing/msolineformathelper/dashstyle/) { get; set; } | Obtient ou définit le style de tiret pour la ligne spécifiée. |
| [ForeColor](../../aspose.cells.drawing/msolineformathelper/forecolor/) { get; set; } | Obtient et définit la couleur de premier plan de la ligne de bordure. |
| [IsVisible](../../aspose.cells.drawing/msolineformathelper/isvisible/) { get; set; } | Indique si l'objet est visible. |
| [Style](../../aspose.cells.drawing/msolineformathelper/style/) { get; set; } | Renvoie un objet Style qui représente le style de la plage spécifiée. |
| [Transparency](../../aspose.cells.drawing/msolineformathelper/transparency/) { get; set; } | Renvoie ou définit le degré de transparence du remplissage spécifié sous forme d'une valeur comprise entre 0.0 (opaque) et 1.0 (transparent). |
| [Weight](../../aspose.cells.drawing/msolineformathelper/weight/) { get; set; } | Renvoie ou définit l'épaisseur de la ligne, en unités de pt. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DrawingClassMsoLineFormatHelperDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Créer une forme pour démontrer le formatage de ligne
                Shape shape = worksheet.Shapes.AddLine(10, 10, 100, 100, 0, 0);

                // Obtenez le format de ligne directement à partir de la forme
                MsoLineFormat lineFormat = shape.LineFormat;

                // Définissez les propriétés directement sur le format de ligne
                lineFormat.IsVisible = true;
                lineFormat.Style = MsoLineStyle.Single;
                lineFormat.ForeColor = Color.Blue;
                lineFormat.BackColor = Color.LightGray;
                lineFormat.DashStyle = MsoLineDashStyle.Solid;
                lineFormat.Transparency = 0.2;
                lineFormat.Weight = 2.5;

                // Affichez les propriétés configurées
                Console.WriteLine($"Line is visible: {lineFormat.IsVisible}");
                Console.WriteLine($"Line style: {lineFormat.Style}");
                Console.WriteLine($"Fore color: {lineFormat.ForeColor}");
                Console.WriteLine($"Back color: {lineFormat.BackColor}");
                Console.WriteLine($"Dash style: {lineFormat.DashStyle}");
                Console.WriteLine($"Transparency: {lineFormat.Transparency}");
                Console.WriteLine($"Weight: {lineFormat.Weight}");

                // Enregistrez le classeur
                workbook.Save("MsoLineFormatHelperDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with MsoLineFormatHelper: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


