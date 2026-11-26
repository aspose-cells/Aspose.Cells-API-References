---
title: "PictureBulletValue.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PictureBulletValue. Obtiene el tipo del valor de la viñeta"
type: docs
url: /es/net/aspose.cells.drawing.texts/picturebulletvalue/type/
---
## PictureBulletValue.Type property

Obtiene el tipo del valor de la viñeta.

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

    public class PictureBulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Crear una instancia de PictureBulletValue
                PictureBulletValue bulletValue = new PictureBulletValue();
                
                // Mostrar el valor de la propiedad Type (operación solo lectura)
                Console.WriteLine("PictureBulletValue Type: " + bulletValue.Type);
                
                // Demostrar que el Type se establece correctamente a Picture para esta clase
                if (bulletValue.Type == BulletType.Picture)
                {
                    Console.WriteLine("Type is correctly set to Picture for PictureBulletValue");
                }
                
                // Guarda el libro de trabajo
                workbook.Save("PictureBulletValueTypeDemo.xlsx");
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
* class [PictureBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


