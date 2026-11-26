---
title: "Clase NoneBulletValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Texts.NoneBulletValue. Representa ninguna viñeta"
type: docs
url: /es/net/aspose.cells.drawing.texts/nonebulletvalue/
---
## NoneBulletValue class

Representa sin viñeta.

```csharp
public class NoneBulletValue : BulletValue
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [NoneBulletValue](nonebulletvalue/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| override [Type](../../aspose.cells.drawing.texts/nonebulletvalue/type/) { get; } | Obtiene el tipo del valor de la viñeta. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class NoneBulletValueDemo
    {
        public static void NoneBulletValueExample()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar texto a una celda
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample text without bullet");

            // Crear un TextBox para aplicar la configuración de viñetas
            Aspose.Cells.Drawing.TextBox textBox = worksheet.TextBoxes[worksheet.TextBoxes.Add(2, 1, 100, 400)];
            textBox.Text = "This is a TextBox without bullet points";

            // Crear una instancia de NoneBulletValue
            NoneBulletValue noneBulletValue = new NoneBulletValue();

            // Verificar el tipo de viñeta (debería ser None)
            BulletType bulletType = noneBulletValue.Type;
            Console.WriteLine("Bullet Type: " + bulletType); // Output should be None

            // Guardar el libro de trabajo para demostrar los cambios
            workbook.Save("NoneBulletValueExample.xlsx");
        }
    }
}
```

### Ver también

* class [BulletValue](../bulletvalue/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


