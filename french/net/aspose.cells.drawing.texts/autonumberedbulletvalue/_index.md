---
title: "Classe AutoNumberedBulletValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.Texts.AutoNumberedBulletValue. Représente une puce numérotée automatique"
type: docs
url: /fr/net/aspose.cells.drawing.texts/autonumberedbulletvalue/
---
## AutoNumberedBulletValue class

Représente une puce numérotée automatique.

```csharp
public class AutoNumberedBulletValue : BulletValue
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [AutoNumberedBulletValue](autonumberedbulletvalue/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [AutonumberScheme](../../aspose.cells.drawing.texts/autonumberedbulletvalue/autonumberscheme/) { get; set; } | Représente le schéma du numéro automatique. |
| [StartAt](../../aspose.cells.drawing.texts/autonumberedbulletvalue/startat/) { get; set; } | Obtient et définit le numéro de départ de la puce. |
| override [Type](../../aspose.cells.drawing.texts/autonumberedbulletvalue/type/) { get; } | Obtient le type de la puce. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassAutoNumberedBulletValueDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Créez une instance AutoNumberedBulletValue
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue
                {
                    AutonumberScheme = TextAutonumberScheme.AlphaUcPeriod,
                    StartAt = 1
                };

                // Affichez les propriétés de la puce
                Console.WriteLine($"Bullet Type: {bullet.Type}");
                Console.WriteLine($"Autonumber Scheme: {bullet.AutonumberScheme}");
                Console.WriteLine($"Starting Number: {bullet.StartAt}");

                // Modifier les propriétés
                bullet.AutonumberScheme = TextAutonumberScheme.ArabicParenR;
                bullet.StartAt = 5;

                // Enregistrez le classeur
                workbook.Save("TextsClassAutoNumberedBulletValueDemo.xlsx");
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

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


