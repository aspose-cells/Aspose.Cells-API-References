---
title: "CharacterBulletValue.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CharacterBulletValue. Получает тип маркера"
type: docs
url: /ru/net/aspose.cells.drawing.texts/characterbulletvalue/type/
---
## CharacterBulletValue.Type property

Получает тип маркера.

```csharp
public override BulletType Type { get; }
```

### Примеры

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
                // Создать новый экземпляр CharacterBulletValue
                CharacterBulletValue bulletValue = new CharacterBulletValue();
                
                // Продемонстрируйте свойство Type (только для чтения)
                Console.WriteLine("Bullet Type: " + bulletValue.Type);
                
                // Показать, что Type является Character для CharacterBulletValue
                Console.WriteLine("Is Character bullet type: " + 
                    (bulletValue.Type == BulletType.Character));
                
                // Продемонстрировать установку свойства Character (чтение-запись)
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

### См. также

* enum [BulletType](../../bullettype/)
* class [CharacterBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


