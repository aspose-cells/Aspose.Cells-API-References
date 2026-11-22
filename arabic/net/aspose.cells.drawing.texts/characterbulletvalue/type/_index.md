---
title: "CharacterBulletValue.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CharacterBulletValue. تحصل على نوع التعداد"
type: docs
url: /ar/net/aspose.cells.drawing.texts/characterbulletvalue/type/
---
## CharacterBulletValue.Type property

يحصل على نوع الرصاصة.

```csharp
public override BulletType Type { get; }
```

### أمثلة

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
                // إنشاء نسخة جديدة من CharacterBulletValue
                CharacterBulletValue bulletValue = new CharacterBulletValue();
                
                // عرض خاصية Type (للقراءة فقط)
                Console.WriteLine("Bullet Type: " + bulletValue.Type);
                
                // أظهر أن النوع هو Character لـ CharacterBulletValue
                Console.WriteLine("Is Character bullet type: " + 
                    (bulletValue.Type == BulletType.Character));
                
                // وضح تعيين خاصية Character (قراءة-كتابة)
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

### انظر أيضًا

* enum [BulletType](../../bullettype/)
* class [CharacterBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


