---
title: "Bullet.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Bullet. Obtient et définit le type de puce"
type: docs
url: /fr/net/aspose.cells.drawing.texts/bullet/type/
---
## Bullet.Type property

Obtient et définit le type de bullet.

```csharp
public BulletType Type { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class BulletPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter une zone de texte
            int textboxIndex = worksheet.TextBoxes.Add(2, 1, 160, 200);
            TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.Text = "Sample text with bullet";

            // Configurer les propriétés de la puce
            Bullet bullet = textbox.TextBody.TextParagraphs[0].Bullet;
            bullet.Type = BulletType.Character; // Demonstrating Type property usage
            ((CharacterBulletValue)bullet.BulletValue).Character = '•';
            bullet.FontName = "Arial";

            // Enregistrez le classeur
            workbook.Save("BulletPropertyTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [BulletType](../../bullettype/)
* class [Bullet](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


