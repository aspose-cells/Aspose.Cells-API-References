---
title: "CharacterBulletValue.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CharacterBulletValue. Obtiene el tipo de la viñeta"
type: docs
url: /es/net/aspose.cells.drawing.texts/characterbulletvalue/type/
---
## CharacterBulletValue.Type property

Obtiene el tipo de la viñeta.

```csharp
public override BulletType Type { get; }
```

### Ejemplos

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
                // Crear una nueva instancia de CharacterBulletValue
                CharacterBulletValue bulletValue = new CharacterBulletValue();
                
                // Demuestra la propiedad Type (solo lectura)
                Console.WriteLine("Bullet Type: " + bulletValue.Type);
                
                // Mostrar que el Tipo es Character para CharacterBulletValue
                Console.WriteLine("Is Character bullet type: " + 
                    (bulletValue.Type == BulletType.Character));
                
                // Demostrar la configuración de la propiedad Character (lectura-escritura)
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

### Ver también

* enum [BulletType](../../bullettype/)
* class [CharacterBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


