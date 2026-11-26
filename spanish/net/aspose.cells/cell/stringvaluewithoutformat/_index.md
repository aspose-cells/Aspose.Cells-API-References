---
title: "Cell.StringValueWithoutFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cell. Obtiene el valor de la celda como cadena sin ningún formato"
type: docs
url: /es/net/aspose.cells/cell/stringvaluewithoutformat/
---
## Cell.StringValueWithoutFormat property

Obtiene el valor de la celda como cadena sin ningún formato.

```csharp
[Obsolete("Use GetStringValue(CellValueFormatStrategy) with CellValueFormatStrategy.None instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StringValueWithoutFormat { get; }
```

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, el usuario debe obtener el objeto de valor y formatearlo según el tipo de valor y el requisito específico. Esta propiedad será eliminada 12 meses después, a partir de diciembre de 2020. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyStringValueWithoutFormatDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar diferentes tipos de datos para demostrar StringValueWithoutFormat
            worksheet.Cells["A1"].PutValue("Plain Text");
            worksheet.Cells["A2"].PutValue(12345);
            worksheet.Cells["A3"].PutValue(3.14159);
            worksheet.Cells["A4"].PutValue(DateTime.Now);

            // Aplicar formato numérico a algunas celdas
            Style style = worksheet.Cells["A2"].GetStyle();
            style.Number = 3; // Currency format
            worksheet.Cells["A2"].SetStyle(style);

            style = worksheet.Cells["A3"].GetStyle();
            style.Number = 9; // Percentage format
            worksheet.Cells["A3"].SetStyle(style);

            try
            {
                // Mostrar StringValueWithoutFormat para cada celda
                Console.WriteLine("A1 StringValueWithoutFormat: " + worksheet.Cells["A1"].StringValueWithoutFormat);
                Console.WriteLine("A2 StringValueWithoutFormat: " + worksheet.Cells["A2"].StringValueWithoutFormat);
                Console.WriteLine("A3 StringValueWithoutFormat: " + worksheet.Cells["A3"].StringValueWithoutFormat);
                Console.WriteLine("A4 StringValueWithoutFormat: " + worksheet.Cells["A4"].StringValueWithoutFormat);

                // Comparar con StringValue formateado
                Console.WriteLine("\nComparison with formatted values:");
                Console.WriteLine("A2 StringValue (formatted): " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("A3 StringValue (formatted): " + worksheet.Cells["A3"].StringValue);

                // Guarda el libro de trabajo
                workbook.Save("StringValueWithoutFormatDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
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

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


