---
title: "Classe NoneBulletValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.Texts.NoneBulletValue. Représente aucune puce"
type: docs
url: /fr/net/aspose.cells.drawing.texts/nonebulletvalue/
---
## NoneBulletValue class

Représente aucune puce.

```csharp
public class NoneBulletValue : BulletValue
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [NoneBulletValue](nonebulletvalue/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| override [Type](../../aspose.cells.drawing.texts/nonebulletvalue/type/) { get; } | Obtient le type de la valeur de la puce. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class NoneBulletValueDemo
    {
        public static void NoneBulletValueExample()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajout de texte à une cellule
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample text without bullet");

            // Créer une TextBox pour appliquer les paramètres de puce
            Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[worksheet.TextBoxes.Add(2, 1, 100, 400)];
            textBox.Text = "This is a TextBox without bullet points";

            // Créer une instance de NoneBulletValue
            NoneBulletValue noneBulletValue = new NoneBulletValue();

            // Vérifier le type de la puce (devrait être None)
            BulletType bulletType = noneBulletValue.Type;
            Console.WriteLine("Bullet Type: " + bulletType); // Output should be None

            // Enregistrer le classeur pour démontrer les modifications
            workbook.Save("NoneBulletValueExample.xlsx");
        }
    }
}
```

### Voir aussi

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


