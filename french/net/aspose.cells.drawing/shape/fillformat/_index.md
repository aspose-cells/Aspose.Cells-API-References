---
title: "Shape.FillFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Retourne un objet MsoFillFormat qui contient les propriétés de mise en forme de remplissage pour la forme spécifiée"
type: docs
url: /fr/net/aspose.cells.drawing/shape/fillformat/
---
## Shape.FillFormat property

Retourne un objet MsoFillFormat qui contient les propriétés de mise en forme de remplissage pour la forme spécifiée.

```csharp
[Obsolete("Use Shape.Fill property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoFillFormat FillFormat { get; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la propriété Shape.Fill. Cette propriété sera supprimée 12 mois plus tard depuis juillet 2016. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyFillFormatDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez une forme rectangulaire pour démontrer la propriété FillFormat
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 100);

            try
            {
                // Accédez à la propriété FillFormat (lecture seule)
                MsoFillFormat fillFormat = shape.FillFormat;

                // Affichez les propriétés FillFormat actuelles
                Console.WriteLine("FillFormat ForeColor: " + fillFormat.ForeColor);
                Console.WriteLine("FillFormat Transparency: " + fillFormat.Transparency);
                Console.WriteLine("FillFormat BackColor: " + fillFormat.BackColor);
                Console.WriteLine("FillFormat IsVisible: " + fillFormat.IsVisible);

                // Modifiez les propriétés FillFormat (puisqu'elle n'est pas en lecture seule)
                fillFormat.ForeColor = System.Drawing.Color.Red;
                fillFormat.Transparency = 0.5;
                fillFormat.BackColor = System.Drawing.Color.Yellow;
                fillFormat.IsVisible = true;

                // Affichez les propriétés FillFormat mises à jour
                Console.WriteLine("Updated FillFormat ForeColor: " + fillFormat.ForeColor);
                Console.WriteLine("Updated FillFormat Transparency: " + fillFormat.Transparency);
                Console.WriteLine("Updated FillFormat BackColor: " + fillFormat.BackColor);
                Console.WriteLine("Updated FillFormat IsVisible: " + fillFormat.IsVisible);

                // Enregistrez le classeur
                workbook.Save("FillFormatDemo.xlsx");
                Console.WriteLine("FillFormat has been demonstrated and workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [MsoFillFormat](../../msofillformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


