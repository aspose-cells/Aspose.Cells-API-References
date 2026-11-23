---
title: "BulletValue.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BulletValue. Obtient le type de la valeur des puces"
type: docs
url: /fr/net/aspose.cells.drawing.texts/bulletvalue/type/
---
## BulletValue.Type property

Obtient le type de la valeur de la puce.

```csharp
public abstract BulletType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class BulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Créer une zone de texte et obtenir ses paragraphes de texte
                var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
                var textParagraph = textBox.TextBody.TextParagraphs[0];

                // Créer une valeur de puce de caractère (qui hérite de BulletValue)
                var bulletValue = new CharacterBulletValue();
                bulletValue.Character = '•';

                // Afficher la valeur de la propriété Type
                Console.WriteLine("Bullet Type: " + bulletValue.Type);

                // Créer une valeur de puce d'image pour afficher un type différent
                var pictureBullet = new PictureBulletValue();
                Console.WriteLine("Picture Bullet Type: " + pictureBullet.Type);

                // Enregistrez le classeur
                workbook.Save("BulletValueTypeDemo.xlsx");
                Console.WriteLine("Type property demonstration completed successfully.");
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

* enum [BulletType](../../bullettype/)
* class [BulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


