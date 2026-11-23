---
title: "AutoNumberedBulletValue.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété AutoNumberedBulletValue. Obtient le type de la puce"
type: docs
url: /fr/net/aspose.cells.drawing.texts/autonumberedbulletvalue/type/
---
## AutoNumberedBulletValue.Type property

Obtient le type de la puce.

```csharp
public override BulletType Type { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créez une forme pour ajouter du texte avec des puces
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 10, 300, 100);
            var textParagraph = shape.TextBody.TextParagraphs[0];

            // Créez une valeur de puce auto-numérotée
            var bullet = new AutoNumberedBulletValue
            {
                AutonumberScheme = TextAutonumberScheme.AlphaLcParenBoth,
                StartAt = 1
            };

            // Puisque nous ne pouvons pas définir BulletValue directement, nous devrons trouver une autre solution
            // pour appliquer le style de puce. Cela peut impliquer l'utilisation du formatage du texte de la forme
            // ou d'autres méthodes disponibles dans l'API.
            // À titre de démonstration, nous afficherons simplement le type de puce
            Console.WriteLine("Bullet Type: " + bullet.Type);

            // Ajoutez du texte au paragraphe via le corps de texte de la forme
            shape.TextBody.Text = "First Item";

            // Ajoutez un autre paragraphe avec un schéma de numérotation différent
            // Puisque nous ne pouvons pas Add, nous utiliserons le paragraphe suivant disponible
            var secondParagraph = shape.TextBody.TextParagraphs[1];
            var bullet2 = new AutoNumberedBulletValue
            {
                AutonumberScheme = TextAutonumberScheme.Arabic1Minus,
                StartAt = 1
            };

            // Afficher le type de puce (propriété en lecture seule)
            Console.WriteLine("Second Bullet Type: " + bullet2.Type);

            // Ajouter du texte au deuxième paragraphe
            shape.TextBody.Text += "\nSecond Item";

            // Enregistrer le classeur pour démontrer les effets de puce
            workbook.Save("AutoNumberedBulletDemo.xlsx");
        }
    }

}
```

### Voir aussi

* enum [BulletType](../../bullettype/)
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


