---
title: "UnionRange.PutValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método UnionRange. Inserta un valor en el rango; si es apropiado, el valor se convertirá a otro tipo de datos y el formato numérico de las celdas se restablecerá"
type: docs
url: /es/net/aspose.cells/unionrange/putvalue/
---
## UnionRange.PutValue method

Inserta un valor en el rango; si es apropiado, el valor se convertirá a otro tipo de datos y se restablecerá el formato numérico de la celda.

```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stringValue | String | Valor de entrada |
| isConverted | Booleano | True: convertido a otro tipo de datos si es apropiado. |
| setStyle | Booleano | True: establecer el formato numérico al estilo de la celda al convertir a otro tipo de datos |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodPutValueWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un rango de unión que cubra las celdas A1 a B2
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });
            
            try
            {
                // Llamar a PutValue con los parámetros: (String, Boolean, Boolean)
                unionRange.PutValue("Sample Value", true, true);
                
                Console.WriteLine("PutValue method executed successfully with parameters (String, Boolean, Boolean)");
                
                // Mostrar la información del rango para mostrar el efecto
                Console.WriteLine($"Range address: {unionRange.RefersTo}");
                Console.WriteLine($"Value set in range: {unionRange.Value}");
                
                // Aplicar formato para que el efecto sea visible
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                style.HorizontalAlignment = TextAlignmentType.Center;
                unionRange.SetStyle(style);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing PutValue method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("UnionRangeMethodPutValueWithStringBooleanBooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


