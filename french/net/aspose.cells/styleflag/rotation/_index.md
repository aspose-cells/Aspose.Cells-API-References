---
title: "StyleFlag.Rotation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété StyleFlag. Le paramètre de rotation sera appliqué"
type: docs
url: /fr/net/aspose.cells/styleflag/rotation/
---
## StyleFlag.Rotation property

Le paramètre de rotation sera appliqué.

```csharp
public bool Rotation { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyRotationDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Accéder à la cellule A1 et définir du texte
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Rotated Text");

            // Obtenir le style de la cellule
            Style style = workbook.CreateStyle();

            // Définir une nouvelle valeur de rotation (45 degrés)
            style.RotationAngle = 45;

            // Afficher la valeur de rotation actuelle
            Console.WriteLine("Current Rotation value: " + cell.GetStyle().RotationAngle);            

            // Créer un indicateur de style et activer l'indicateur de rotation
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Rotation = true;

            // Appliquer le style avec rotation à la cellule
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("after setting style, rotation value: " + cell.GetStyle().RotationAngle);
           
            // Enregistrer le résultat
            workbook.Save("PropertyRotationDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


