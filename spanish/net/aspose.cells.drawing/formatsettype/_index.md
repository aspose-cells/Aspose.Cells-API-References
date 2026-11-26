---
title: "Enumeración FormatSetType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.FormatSetType. Tipo de conjunto de formato de relleno"
type: docs
url: /es/net/aspose.cells.drawing/formatsettype/
---
## FormatSetType enumeration

Tipo de conjunto de formato de relleno.

```csharp
public enum FormatSetType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Sin formato de relleno. |
| IsGradientSet | `1` | Formato de relleno degradado. |
| IsTextureSet | `2` | Formato de relleno de textura. |
| IsPatternSet | `3` | Formato de relleno de patrón. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassFormatSetTypeDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar una forma para demostrar el formato de relleno
                Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 200);
                FillFormat fillFormat = shape.Fill;

                // Mostrar tipo de relleno inicial
                Console.WriteLine("Initial fill type: " + fillFormat.Type);

                // Demostrar valores de la enumeración FormatSetType
                Console.WriteLine("FormatSetType.None: " + (int)FormatSetType.None);
                Console.WriteLine("FormatSetType.IsGradientSet: " + (int)FormatSetType.IsGradientSet);
                Console.WriteLine("FormatSetType.IsTextureSet: " + (int)FormatSetType.IsTextureSet);
                Console.WriteLine("FormatSetType.IsPatternSet: " + (int)FormatSetType.IsPatternSet);

                // Aplicar diferentes tipos de relleno usando FormatSetType
                fillFormat.Type = (FillType)FormatSetType.IsGradientSet;
                Console.WriteLine("After setting gradient: " + fillFormat.Type);

                fillFormat.Type = (FillType)FormatSetType.IsPatternSet;
                Console.WriteLine("After setting pattern: " + fillFormat.Type);

                // Guarda el libro de trabajo
                workbook.Save("FormatSetTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with FormatSetType: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


