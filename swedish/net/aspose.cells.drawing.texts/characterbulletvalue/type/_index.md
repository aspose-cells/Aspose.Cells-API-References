---
title: "CharacterBulletValue.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CharacterBulletValue‑egenskap. Hämtar typen av bullet"
type: docs
url: /sv/net/aspose.cells.drawing.texts/characterbulletvalue/type/
---
## CharacterBulletValue.Type property

Hämtar typen av punkten.

```csharp
public override BulletType Type { get; }
```

### Exempel

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
                // Skapa en ny CharacterBulletValue‑instans
                CharacterBulletValue bulletValue = new CharacterBulletValue();
                
                // Demonstrera Type-egenskapen (skrivskyddad)
                Console.WriteLine("Bullet Type: " + bulletValue.Type);
                
                // Visa att Type är Character för CharacterBulletValue
                Console.WriteLine("Is Character bullet type: " + 
                    (bulletValue.Type == BulletType.Character));
                
                // Demonstrera att sätta Character‑egenskapen (läs- och skrivbar)
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

### Se även

* enum [BulletType](../../bullettype/)
* class [CharacterBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


