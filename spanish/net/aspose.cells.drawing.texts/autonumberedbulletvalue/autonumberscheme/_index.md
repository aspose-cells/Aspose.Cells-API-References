---
title: "AutoNumberedBulletValue.AutonumberScheme"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad AutoNumberedBulletValue. Representa el esquema de numeración automática"
type: docs
url: /es/net/aspose.cells.drawing.texts/autonumberedbulletvalue/autonumberscheme/
---
## AutoNumberedBulletValue.AutonumberScheme property

Representa el esquema de numeración automática.

```csharp
public TextAutonumberScheme AutonumberScheme { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyAutonumberSchemeDemo
    {
        public static void Run()
        {
            try
            {
                // Crear una nueva instancia de AutoNumberedBulletValue
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue();

                // Mostrar el valor inicial de AutonumberScheme
                Console.WriteLine($"Default AutonumberScheme: {bullet.AutonumberScheme}");

                // Establecer un nuevo valor de AutonumberScheme
                bullet.AutonumberScheme = TextAutonumberScheme.RomanUcPeriod;
                Console.WriteLine($"Modified AutonumberScheme: {bullet.AutonumberScheme}");

                // Crear un libro de trabajo para demostrar la viñeta en contexto
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Crear una forma con texto que utilizará el estilo de viñeta
                TextBox shape = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 100);
                shape.TextBody.Text = "Sample text with bullet formatting";


                // Nota: La aplicación real del estilo de viñeta al texto requeriría llamadas adicionales a la API
                // No se muestra en la reflexión. Simplemente guardaremos el libro de trabajo como demostración.
                workbook.Save("AutonumberSchemeDemo.xlsx");
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

* enum [TextAutonumberScheme](../../textautonumberscheme/)
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


