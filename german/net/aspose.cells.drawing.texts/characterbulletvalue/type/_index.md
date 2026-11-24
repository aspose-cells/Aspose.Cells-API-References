---
title: "CharacterBulletValue.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CharacterBulletValue-Eigenschaft. Gibt den Typ der Aufzählung zurück"
type: docs
url: /de/net/aspose.cells.drawing.texts/characterbulletvalue/type/
---
## CharacterBulletValue.Type property

Liest den Typ der Aufzählung.

```csharp
public override BulletType Type { get; }
```

### Beispiele

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
                // Erstelle eine neue Instanz von CharacterBulletValue
                CharacterBulletValue bulletValue = new CharacterBulletValue();
                
                // Demonstriere die Type-Eigenschaft (schreibgeschützt)
                Console.WriteLine("Bullet Type: " + bulletValue.Type);
                
                // Zeige, dass der Typ für CharacterBulletValue 'Character' ist
                Console.WriteLine("Is Character bullet type: " + 
                    (bulletValue.Type == BulletType.Character));
                
                // Demonstriere das Setzen der Character-Eigenschaft (les- und schreibbar)
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

### Siehe auch

* enum [BulletType](../../bullettype/)
* class [CharacterBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


