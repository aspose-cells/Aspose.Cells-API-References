---
title: "CharacterBulletValue.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà CharacterBulletValue. Ottiene il tipo dell'elenco puntato"
type: docs
url: /it/net/aspose.cells.drawing.texts/characterbulletvalue/type/
---
## CharacterBulletValue.Type property

Ottiene il tipo del punto elenco.

```csharp
public override BulletType Type { get; }
```

### Esempi

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
                // Crea una nuova istanza di CharacterBulletValue
                CharacterBulletValue bulletValue = new CharacterBulletValue();
                
                // Dimostra la proprietà Type (sola lettura)
                Console.WriteLine("Bullet Type: " + bulletValue.Type);
                
                // Mostra che il Tipo è Character per CharacterBulletValue
                Console.WriteLine("Is Character bullet type: " + 
                    (bulletValue.Type == BulletType.Character));
                
                // Dimostra l'impostazione della proprietà Character (lettura-scrittura)
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

### Vedi anche

* enum [BulletType](../../bullettype/)
* class [CharacterBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


