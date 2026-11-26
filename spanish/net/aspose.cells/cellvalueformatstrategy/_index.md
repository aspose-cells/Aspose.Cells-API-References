---
title: "Enumeración CellValueFormatStrategy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.CellValueFormatStrategy. Especifica cómo aplicar el estilo al valor de la celda"
type: docs
url: /es/net/aspose.cells/cellvalueformatstrategy/
---
## CellValueFormatStrategy enumeration

Especifica cómo aplicar el estilo al valor de la celda.

```csharp
public enum CellValueFormatStrategy
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | No formateado. |
| CellStyle | `1` | Solo formateado con el estilo original de la celda. |
| DisplayStyle | `2` | Formateado con el estilo mostrado de la celda. |
| DisplayString | `3` | Obtiene la cadena mostrada en MS Excel. La principal diferencia con DisplayStyle es que esta opción también considera el efecto del ancho de columna. Si el ancho de columna es demasiado pequeño para mostrar la cadena formateada completamente, puede mostrarse \"#\", al igual que lo hace MS Excel. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueFormatStrategyDemo
    {
        public static void CellValueFormatStrategyExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B1"].PutValue("Number");
            worksheet.Cells["B2"].PutValue(12345.6789);
            worksheet.Cells["C1"].PutValue("Text");
            worksheet.Cells["C2"].PutValue("Hello World");

            // Aplica diferentes CellValueFormatStrategy para demostrar sus efectos
            // Ninguno: No formateado
            string valueNone = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.None);
            Console.WriteLine($"None: {valueNone}");

            // CellStyle: Solo formateado con el estilo original de la celda
            string valueCellStyle = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.CellStyle);
            Console.WriteLine($"CellStyle: {valueCellStyle}");

            // DisplayStyle: Formateado con el estilo mostrado de la celda
            string valueDisplayStyle = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.DisplayStyle);
            Console.WriteLine($"DisplayStyle: {valueDisplayStyle}");

            // DisplayString: Obtiene la cadena mostrada en MS Excel
            string valueDisplayString = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.DisplayString);
            Console.WriteLine($"DisplayString: {valueDisplayString}");

            // Guardar el libro de trabajo en un archivo
            workbook.Save("CellValueFormatStrategyExample.xlsx");
            workbook.Save("CellValueFormatStrategyExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


