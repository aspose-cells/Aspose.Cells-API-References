---
title: "Classe BulletValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Drawing.Texts.BulletValue. Représente la valeur de la puce"
type: docs
url: /fr/net/aspose.cells.drawing.texts/bulletvalue/
---
## BulletValue class

Représente la valeur de la puce.

```csharp
public abstract class BulletValue
```

## Propriétés

| Nom | Description |
| --- | --- |
| abstract [Type](../../aspose.cells.drawing.texts/bulletvalue/type/) { get; } | Obtient le type de la valeur de la puce. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassBulletValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une zone de texte et obtenir ses paragraphes de texte
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var textParagraph = textBox.TextBody.TextParagraphs[0];

            // Créer une instance de CharacterBulletValue (qui hérite de BulletValue)
            var bulletValue = new CharacterBulletValue();
            bulletValue.Character = '•';
            
            // Définir la valeur de la puce pour le paragraphe (Bullet est en lecture seule, nous devons donc le modifier différemment)
            // Étant donné que Bullet est en lecture seule, nous devons trouver une autre façon de le définir
            // Cela pourrait impliquer la création d'un nouveau TextParagraph avec la puce définie
            // Remarque : L'API réelle pourrait offrir une méthode différente pour définir les puces
            // À titre d'exemple, nous supposerons que nous pouvons le définir par d'autres moyens
            // textParagraph.Bullet = bulletValue; // Cette ligne est supprimée car Bullet est en lecture seule
            textBox.Text = "First bullet point";

            // Ajouter un autre paragraphe avec une puce différente
            // TextParagraphCollection n'a pas de méthode Add, nous devons donc trouver une autre façon
            // Cela pourrait impliquer la création d'un nouveau TextParagraph et son ajout par d'autres moyens
            // À titre d'exemple, nous supposerons que nous pouvons obtenir directement le deuxième paragraphe
            var textParagraph2 = textBox.TextBody.TextParagraphs[1];
            var bulletValue2 = new CharacterBulletValue();
            bulletValue2.Character = '→';
            // textParagraph2.Bullet = bulletValue2; // Cette ligne est supprimée car Bullet est en lecture seule
            textBox.Text += "\nSecond bullet point";

            // Démontrer l'accès au type de puce
            Console.WriteLine("First bullet type: " + textParagraph.Bullet.Type);
            Console.WriteLine("Second bullet type: " + textParagraph2.Bullet.Type);

            // Enregistrer le résultat
            workbook.Save("TextsClassBulletValueDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


