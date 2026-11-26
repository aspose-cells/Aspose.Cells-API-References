---
title: "Enum CellsUnitType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.CellsUnitType. Especifica la unidad de medida"
type: docs
url: /es/net/aspose.cells/cellsunittype/
---
## CellsUnitType enumeration

Especifica la unidad de medida.

```csharp
public enum CellsUnitType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Pixel | `1` | La medida está en píxeles. |
| Point | `2` | La medida está en puntos. Un punto representa 1/72 de pulgada. |
| Inch | `4` | La medida está en pulgadas. |
| Cm | `6` | La medida está en centímetros. |
| Character | `7` | En unidades de caracteres. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCellsUnitTypeDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Demuestra el uso de diferentes valores del enum CellsUnitType
                Console.WriteLine("Available CellsUnitType values:");

                // Muestra todos los valores del enum
                Console.WriteLine("Pixel: " + CellsUnitType.Pixel);
                Console.WriteLine("Point: " + CellsUnitType.Point);
                Console.WriteLine("Inch: " + CellsUnitType.Inch);
                Console.WriteLine("Cm: " + CellsUnitType.Cm);
                Console.WriteLine("Character: " + CellsUnitType.Character);

                // Ejemplo de uso: Establece el ancho de columna usando diferentes unidades
                worksheet.Cells.SetColumnWidthPixel(0, 100); // Using Pixel unit
                worksheet.Cells.SetColumnWidthInch(1, 2.0);  // Using Inch unit

                // Guarda el libro de trabajo para demostrar un flujo completo
                workbook.Save("CellsUnitTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with different unit types applied.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with CellsUnitType: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


