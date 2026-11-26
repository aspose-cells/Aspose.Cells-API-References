---
title: "FontConfigs.IsFontAvailable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método FontConfigs. Indica si la fuente está disponible"
type: docs
url: /es/net/aspose.cells/fontconfigs/isfontavailable/
---
## FontConfigs.IsFontAvailable method

Indique si la fuente está disponible.

```csharp
public static bool IsFontAvailable(string fontName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontName | String | nombre de fuente |

### Valor de retorno

true si la fuente está disponible, de lo contrario false.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodIsFontAvailableWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Probar nombres de fuentes para comprobar disponibilidad
            string[] testFonts = { "Arial", "Times New Roman", "NonExistentFont" };

            try
            {
                foreach (string fontName in testFonts)
                {
                    // Llamar al método IsFontAvailable con el nombre de la fuente
                    bool isAvailable = FontConfigs.IsFontAvailable(fontName);

                    // Mostrar el resultado
                    Console.WriteLine($"Font '{fontName}' is available: {isAvailable}");

                    // Escribir el resultado en la hoja de cálculo
                    int row = worksheet.Cells.MaxDataRow + 1;
                    worksheet.Cells[row, 0].PutValue($"Font '{fontName}' available:");
                    worksheet.Cells[row, 1].PutValue(isAvailable);
                }

                Console.WriteLine("Method executed successfully with parameters (String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsFontAvailable method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("FontConfigsMethodIsFontAvailableWithStringDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


