---
title: "Fill.Equals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Fill. /"
type: docs
url: /es/net/aspose.cells.drawing/fill/equals/
---
## Fill.Equals method

/

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class FillMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agrega una forma rectangular a la hoja de cálculo
                Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 0, 0, 100, 150);

                // Obtener el objeto FillFormat de la forma
                FillFormat fillFormat1 = rectangle.Fill;

                // Crear otra forma para obtener un segundo objeto FillFormat
                Shape oval = worksheet.Shapes.AddOval(3, 0, 0, 0, 100, 150);
                FillFormat fillFormat2 = oval.Fill;

                // Llamar al método Equals para comparar los dos objetos FillFormat
                bool areEqual = fillFormat1.Equals(fillFormat2);

                // Mostrar el resultado de la comparación
                Console.WriteLine($"FillFormat objects are equal: {areEqual}");

                // También demostrar la comparación con null
                bool isNullEqual = fillFormat1.Equals(null);
                Console.WriteLine($"FillFormat object equals null: {isNullEqual}");

                // Guarda el libro de trabajo
                workbook.Save("FillEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in FillFormat Equals demonstration: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Fill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


