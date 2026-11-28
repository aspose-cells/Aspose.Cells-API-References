---
title: "CharacterBulletValue.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CharacterBulletValue özelliği. Madde işaretinin tipini alır"
type: docs
url: /tr/net/aspose.cells.drawing.texts/characterbulletvalue/type/
---
## CharacterBulletValue.Type property

Madde işaretinin türünü alır.

```csharp
public override BulletType Type { get; }
```

### Örnekler

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
                // Yeni bir CharacterBulletValue örneği oluştur
                CharacterBulletValue bulletValue = new CharacterBulletValue();
                
                // Type özelliğini (yalnızca okuma) gösterin
                Console.WriteLine("Bullet Type: " + bulletValue.Type);
                
                // CharacterBulletValue için Tipin Character olduğunu göster
                Console.WriteLine("Is Character bullet type: " + 
                    (bulletValue.Type == BulletType.Character));
                
                // Character özelliğini ayarlamayı göster (okuma-yazma)
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

### Ayrıca Bakınız

* enum [BulletType](../../bullettype/)
* class [CharacterBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


