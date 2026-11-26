---
title: "AutoNumberedBulletValue.StartAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AutoNumberedBulletValue. Obtiene y establece el número inicial de la viñeta"
type: docs
url: /es/net/aspose.cells.drawing.texts/autonumberedbulletvalue/startat/
---
## AutoNumberedBulletValue.StartAt property

Obtiene y establece el número inicial de la viñeta.

```csharp
public int StartAt { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyStartAtDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Crea una instancia de AutoNumberedBulletValue
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue
                {
                    AutonumberScheme = TextAutonumberScheme.ArabicPeriod,
                    StartAt = 3 // Setting the StartAt property
                };

                // Mostrar el valor actual de StartAt
                Console.WriteLine($"Initial StartAt value: {bullet.StartAt}");

                // Modificar el valor de StartAt
                bullet.StartAt = 5;
                Console.WriteLine($"Modified StartAt value: {bullet.StartAt}");

                // Crear una forma para demostrar la viñeta en contexto
                var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 100);
                shape.TextBody.Text = "1. First Item\n2. Second Item";

                // Aplicar el estilo de viñeta (nota: el método real de aplicación no se muestra en la reflexión)
                // Para la demostración, simplemente guardaremos el libro de trabajo
                workbook.Save("StartAtPropertyDemo.xlsx");
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

* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


