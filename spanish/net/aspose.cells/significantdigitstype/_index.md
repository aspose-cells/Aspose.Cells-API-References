---
title: "Enum SignificantDigitsType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.SignificantDigitsType enum. Representa el tipo de dígitos significativos para la salida de valores numéricos"
type: docs
url: /es/net/aspose.cells/significantdigitstype/
---
## SignificantDigitsType enumeration

Representa el tipo de dígitos significativos para la salida de valores numéricos.

```csharp
public enum SignificantDigitsType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Digits15 | `0` | 15-dígitos |
| G17 | `1` | 17-dígitos formateando el valor con "G17". |
| Rounding17 | `2` | 17-dígitos redondeando el valor. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassSignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Cree un nuevo libro de trabajo para la demostración
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Demuestra el uso de cada valor del enum SignificantDigitsType
                SignificantDigitsType[] types = {
                    SignificantDigitsType.Digits15,
                    SignificantDigitsType.G17,
                    SignificantDigitsType.Rounding17
                };

                foreach (SignificantDigitsType type in types)
                {
                    // Establece el tipo de dígitos significativos para el libro de trabajo
                    workbook.Settings.SignificantDigitsType = type;

                    // Muestra la configuración actual
                    Console.WriteLine($"Current SignificantDigitsType: {type} (Value: {(int)type})");

                    // Añade un valor de muestra para demostrar la configuración
                    worksheet.Cells["A1"].PutValue(123.4567890123456789);

                    // Guarda el libro de trabajo con la configuración actual
                    string fileName = $"SignificantDigitsType_{type}.xlsx";
                    workbook.Save(fileName);
                    Console.WriteLine($"Workbook saved with {type} setting as {fileName}");
                }

                Console.WriteLine("All SignificantDigitsType demonstrations completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating SignificantDigitsType: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


