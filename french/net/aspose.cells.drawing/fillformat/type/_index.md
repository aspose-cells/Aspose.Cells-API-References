---
title: "FillFormat.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FillFormat. Obtient et définit le type de remplissage"
type: docs
url: /fr/net/aspose.cells.drawing/fillformat/type/
---
## FillFormat.Type property

Obtient et définit le type de remplissage.

```csharp
[Obsolete("Use FillFormat.FillType  instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public FillType Type { get; set; }
```

### Remarques

NOTE : Ce membre est maintenant obsolète. Veuillez plutôt utiliser la propriété FillFormat.FillType. Cette propriété sera supprimée 12 mois après juillet 2016. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une forme rectangulaire
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);
            FillFormat fill = shape.Fill;

            // Afficher la valeur actuelle de Type
            Console.WriteLine("Current Type value: " + fill.Type);

            // Modifier Type en Gradient (propriété obsolète utilisée pour la démonstration)
            fill.Type = FillType.Gradient;

            // Appliquer un effet de dégradé à deux couleurs
            fill.SetTwoColorGradient(Color.Blue, Color.Green, GradientStyleType.Horizontal, 1);

            // Enregistrer le classeur modifié
            workbook.Save("FillFormatTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


