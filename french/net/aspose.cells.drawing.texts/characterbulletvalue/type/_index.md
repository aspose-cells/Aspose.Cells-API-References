---
title: "CharacterBulletValue.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CharacterBulletValue. Obtient le type de la puce"
type: docs
url: /fr/net/aspose.cells.drawing.texts/characterbulletvalue/type/
---
## CharacterBulletValue.Type property

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

    public class CharacterBulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Créer une nouvelle instance CharacterBulletValue
                CharacterBulletValue bulletValue = new CharacterBulletValue();
                
                // Démontrez la propriété Type (lecture seule)
                Console.WriteLine("Bullet Type: " + bulletValue.Type);
                
                // Montrer que le Type est Character pour CharacterBulletValue
                Console.WriteLine("Is Character bullet type: " + 
                    (bulletValue.Type == BulletType.Character));
                
                // Démontrer la définition de la propriété Character (lecture-écriture)
                bulletValue.Character = '•';
                Console.WriteLine("Bullet Character: " + bulletValue.Character);
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
* class [CharacterBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


