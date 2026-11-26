---
title: "CellsHelper.SignificantDigitsType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellsHelper. Obtiene y establece el tipo predeterminado de dígitos significativos para la salida de valores numéricos. El valor predeterminado es G17"
type: docs
url: /es/net/aspose.cells/cellshelper/significantdigitstype/
---
## CellsHelper.SignificantDigitsType property

Obtiene y establece el tipo predeterminado de dígitos significativos para la salida de valores numéricos. El valor predeterminado es G17.

```csharp
public static SignificantDigitsType SignificantDigitsType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperPropertySignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Mostrar el valor actual de SignificantDigitsType
                Console.WriteLine("Current SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Establecer un nuevo valor de SignificantDigitsType
                CellsHelper.SignificantDigitsType = SignificantDigitsType.G17;
                Console.WriteLine("Updated SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Crear un libro de trabajo para demostrar el efecto
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Agregar un valor numérico que será afectado por los dígitos significativos
                worksheet.Cells["A1"].PutValue(1.2345678912345678);
                worksheet.Cells["A2"].PutValue(1.2345678912345678);
                worksheet.Cells["A3"].Formula = "=A1+A2";

                // Calcular fórmulas con el tipo actual de dígitos significativos
                workbook.CalculateFormula();

                // Mostrar el resultado
                Console.WriteLine("Calculation result: " + worksheet.Cells["A3"].Value);

                // Cambiar a otro tipo de dígitos significativos
                CellsHelper.SignificantDigitsType = SignificantDigitsType.Rounding17;
                Console.WriteLine("Changed SignificantDigitsType: " + CellsHelper.SignificantDigitsType);

                // Recalcular con el nuevo tipo de dígitos significativos
                workbook.CalculateFormula();
                Console.WriteLine("Recalculated result: " + worksheet.Cells["A3"].Value);

                // Guarda el libro de trabajo
                workbook.Save("SignificantDigitsTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* enum [SignificantDigitsType](../../significantdigitstype/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


